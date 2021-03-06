---

layout: breadcrumbs
permalink: /converter-bots
title: Bots Converter
description: Assisting tool to convert bot entries from collective wiki sheets to wiki pages
breadcrumbs:
  Converter: "/converter"
robots: "NOINDEX, NOFOLLOW"
sitemap: false

---

# Bots WikiSheets Converter


<h2 id="bots">Bots</h2>

<div id="autoconverter-bots">
	<h3>Input</h3>
	<textarea id="input-bots" placeholder="Copy paste a column from the wikisheet here"></textarea>
	<button id="convert-bots">Convert</button>
	<h3>Output</h3>
	<textarea id="output-bots" placeholder="Click &#39;Convert&#39; to generate the output"></textarea>
</div>

<style type="text/css">
#autoconverter-bots textarea {
	width: 100%;
	height: 200px;
}
</style>

<script type="text/javascript">
	
var botRows = ["contributors", "updatedAt", "# Wiki page infos", "title", "name", "description", "imageUrl", "breadcrumbs", "  Bots", "  -_class_-", "# Bot infos", "botName", "botDescription", "botImageUrl", "botType", "botRarity", "botRaritySortOrder", "botAcquisition", "botOpinion", "searchKeywords", "# Abilities infos", "ability1Name", "ability1Info", "ability1Description", "ability2Name", "ability2Info", "ability2Description", "ability3Name", "ability3Info", "ability3Description", "# AI tree infos", "ai1aName", "ai1aDescription", "ai1bName", "ai1bDescription", "ai2aName", "ai2aDescription", "ai2bName", "ai2bDescription", "ai3aName", "ai3aDescription", "ai3bName", "ai3bDescription", "ai4aName", "ai4aDescription", "ai4bName", "ai4bDescription", "ai5aName", "ai5aDescription", "ai5bName", "ai5bDescription", "# Stats infos", "lvl1Hp", "lvl1Dmg", "lvl1Dps", "lvl1Speed", "lvl10Hp", "lvl10Dmg", "lvl10Dps", "lvl20Hp", "lvl20Dmg", "lvl20Dps", "lvl25Hp", "lvl25Dmg", "lvl25Dps", "lvl30Hp", "lvl30Dmg", "lvl30Dps", "# Upgrade infos", "epicMat", "rareMat", "specialMat", "commonMat1", "commonMat2", "commonMat3"]	;

function select(s){
	return s.split('__begin__\n')[1].split('\n__end__')[0]
}
function decorate(s){
	return '---\nlayout: bot\n'+s+'\n---'
}

// Hotfix on top of hot mess because the mobile Sheet app corrupts the clipboard for some reason
// demo: https://cdn.discordapp.com/attachments/923509490307977227/986282674337484881/XRecorder_Edited_14062022_165448.mp4
function fixVal(val){
    if (val.match("''/")){
        val = val.replaceAll("''",'___').replaceAll("'",'').replaceAll('___',"'")
    }
    return val
}
function formatStr(str){
	var i=0;
	return	decorate(
		select(str).replaceAll('"\nhttp', 'http',).split('\n')
			.map(function(line){return line.replaceAll('"','')})
			.map(function(val){return botRows[i++]+': "'+fixVal(val)+'"'})
			.join('\n').replace(/#.*"_?_?"/g,'\n').replaceAll('__','')
		)
}
function convertFromFields(){
	var input = document.querySelector('#input-bots').value;
	var freeform = input.split('__end__').length > 1 ? input.split('__end__')[1] : '';
	var str = formatStr(input);
	var botClass = str.split('botType: "')[1].split('"')[0]
	document.querySelector('#output-bots').value = str.replace('-_class_-: "', botClass+': "').replace('breadcrumbs: ""', 'breadcrumbs:')+'\n\n'+freeform.replace(/^\s*"/,'').replace(/"\s*$/,'')+'\n';
}
document.querySelector('#convert-bots').onclick = convertFromFields;

function trimInput(){
	document.querySelector('#input-bots').value = document.querySelector('#input-bots').value.trim();
	console.log(document.querySelector('#input-bots').value.trim())
}
document.querySelector('#input-bots').addEventListener('input', trimInput, false);
</script>
