---
layout: breadcrumbs
permalink: "/custom-bot"
title: "Custom Bots Builder"
name: "Custom Bots Builder"
description: "Use this Bot Builder to write up and share your custom bots!"
breadcrumbs:
  Community Adventure: "/#community"
---

<style type="text/css">
    .botcard {
        border-radius: 10px;
        width: 240px;
        display: flex;
        flex-direction: column;
        margin: 0 auto;
    }
    .actual-card{
      margin-bottom: 20px;
    }
    .pic {
    background: linear-gradient(160deg, #1b1a6b 50%, cyan);
}
    .cardinfos {
        background: #246eff;
    }
    .cardinfos * {
        font-weight: 1000;
    }
    
    .cardinfos table {
        overflow-x: hidden;
        margin: 0px;
    }
    .bot_bloc_4{
      width: 100%;
    }
</style>

<h3>Custom Bot Builder</h3>
<div>
    <p>Click any text about your bot to edit it live. Then share the link to this page after your edit to share your custom bot (use an <a href="https://tinyurl.com/" target="_blank">url shortener like https://tinyurl.com/</a> or the message will be too big for discord)</p>
</div>

<div class="bot-infos">
    <div class="bot_bloc_1">
        <div class="intro">
            <h1 class="custom-edit custom-edit-name">Custom Bot name...</h1>

            <p><code class="custom-edit custom-edit-desc">Custom Bot description...</code></p>
        </div>
        <div class="botcard">
          <div class="actual-card">
            <div class="pic">
                <p><img loading="lazy" src="/assets/img/icons/cog.png" class="custom-edit custom-edit-image" /></p>
            </div>
            <div class="cardinfos">
                <table>
                  <thead>
                    <tr>
                      <th>Type</th>
                      <th>Rarity</th>
                      <th>Acquisition</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td class="custom-edit custom-edit-class">Class...</td>
                      <td class="custom-edit custom-edit-rarity">Rarity...</td>
                      <td class="custom-edit custom-edit-acquisition">Acquisition...</td>
                    </tr>
                  </tbody>
                </table>
            </div>
          </div>
          <div>
            <h3 id="overview">Overview</h3>
            <div>
              <p class="custom-edit custom-edit-overview">Overview of your bot...</p>
              <p><a href="#comments" title="Comments, AI Builds, tips & tricks...">AI Builds, Tips, etc.</a></p>
            </div>

          </div>
        </div>

        <div class="abilities">
            <h2 id="abilities">Abilities</h2>

            <ul>
              <li>
                <p><h3 class="custom-edit custom-edit-ability1name">1st Ability Name...</h3><code class="custom-edit custom-edit-ability1infos">infos...</code></p>
                <p class="custom-edit custom-edit-ability1desc">description...</p>
              </li>
              <li>
                <p><h3 class="custom-edit custom-edit-ability2name">2st Ability Name...</h3><code class="custom-edit custom-edit-ability2infos">infos...</code></p>
                <p class="custom-edit custom-edit-ability2desc">description...</p>
              </li>
              <li>
                <p><h3 class="custom-edit custom-edit-ability3name">3st Ability Name...</h3><code class="custom-edit custom-edit-ability3infos">infos...</code></p>
                <p class="custom-edit custom-edit-ability3desc">description...</p>
              </li>
            </ul>
        </div>
    </div>

    <div class="bot_bloc_2">

        <h2 id="ai-tree">AI tree</h2>

        <ul>
          <li>
            <p>AI Level 1 (500xp)</p>

            <table>
              <thead>
                <tr>
                  <th class="custom-edit custom-edit-ai1aName">ai1aName...</th>
                  <th class="custom-edit custom-edit-ai1bName">ai1bName...</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td class="custom-edit custom-edit-ai1aDesc">ai1aDescription...</td>
                  <td class="custom-edit custom-edit-ai1bDesc">ai1bDescription...</td>
                </tr>
              </tbody>
            </table>
          </li>
          <li>
            <p>AI Level 2 (2000xp)</p>

            <table>
              <thead>
                <tr>
                  <th class="custom-edit custom-edit-ai2aName">ai2aName...</th>
                  <th class="custom-edit custom-edit-ai2bName">ai2bName...</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td class="custom-edit custom-edit-ai2aDesc">ai2aDescription...</td>
                  <td class="custom-edit custom-edit-ai2bDesc">ai2bDescription...</td>
                </tr>
              </tbody>
            </table>
          </li>
          <li>
            <p>AI Level 3 (5000xp)</p>

            <table>
              <thead>
                <tr>
                  <th class="custom-edit custom-edit-ai3aName">ai3aName...</th>
                  <th class="custom-edit custom-edit-ai3bName">ai3bName...</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td class="custom-edit custom-edit-ai3aDesc">ai3aDescription...</td>
                  <td class="custom-edit custom-edit-ai3bDesc">ai3bDescription...</td>
                </tr>
              </tbody>
            </table>
          </li>
          <li>
            <p>AI Level 4 (14000xp)</p>

            <table>
              <thead>
                <tr>
                  <th class="custom-edit custom-edit-ai4aName">ai4aName...</th>
                  <th class="custom-edit custom-edit-ai4bName">ai4bName...</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td class="custom-edit custom-edit-ai4aDesc">ai4aDescription...</td>
                  <td class="custom-edit custom-edit-ai4bDesc">ai4bDescription...</td>
                </tr>
              </tbody>
            </table>
          </li>
          <li>
            <p>AI Level 5 (30000xp)</p>

            <table>
              <thead>
                <tr>
                  <th class="custom-edit custom-edit-ai5aName">ai5aName...</th>
                  <th class="custom-edit custom-edit-ai5bName">ai5bName...</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td class="custom-edit custom-edit-ai5aDesc">ai5aDescription...</td>
                  <td class="custom-edit custom-edit-ai5bDesc">ai5bDescription...</td>
                </tr>
              </tbody>
            </table>
          </li>
        </ul>
    </div>
    <div class="bot_bloc_3">
        <div class="stats">
            
            <h2 id="stats">Stats</h2>

            <table>
              <thead>
                <tr>
                  <th>Stats</th>
                  <th>Health</th>
                  <th>Attack</th>
                  <th>DPS</th>
                  <th>Speed</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Lvl 1</td>
                  <td class="custom-edit custom-edit-lvl1Hp">lvl1Hp...</td>
                  <td class="custom-edit custom-edit-lvl1Dmg">lvl1Dmg...</td>
                  <td class="custom-edit custom-edit-lvl1Dps">lvl1Dps...</td>
                  <td class="custom-edit custom-edit-lvl1Speed">lvl1Speed...</td>
                </tr>
                <tr>
                  <td>Lvl 10</td>
                  <td> - </td>
                  <td> - </td>
                  <td> - </td>
                  <td> - </td>
                </tr>
                <tr>
                  <td>Lvl 20</td>
                  <td> - </td>
                  <td> - </td>
                  <td> - </td>
                  <td> - </td>
                </tr>
                <tr>
                  <td>Lvl 25</td>
                  <td> - </td>
                  <td> - </td>
                  <td> - </td>
                  <td> - </td>
                </tr>
                <tr>
                  <td>Lvl 30</td>
                  <td class="custom-edit custom-edit-lvl30Hp">lvl30Hp...</td>
                  <td class="custom-edit custom-edit-lvl30Dmg">lvl30Dmg...</td>
                  <td class="custom-edit custom-edit-lvl30Dps">lvl30Dps...</td>
                  <td class="custom-edit custom-edit-lvl30Speed">lvl30Speed...</td>
                </tr>
              </tbody>
            </table>
        </div>

      <div class="bot_bloc_3">
        <h2 id="concept-art">Concept Art</h2>
        <img loading="lazy" src="/assets/img/icons/cog.png" class="custom-edit custom-edit-conceptArt" />
      </div>

      <div class="bot_bloc_4">
        <h2 id="comments">Comments</h2>
          <p class="custom-edit custom-edit-notes">Notes...</p>
        <h3 id="creators">Creators</h3>
          <p class="custom-edit custom-edit-creators">Notes...</p>
        <p>Last updated at: <span class="custom-edit custom-edit-updatedAt"></span></p>
      </div>
</div>


<script type="text/javascript">

    // global state with all the updated values. Serialized/b64 encoded into the anchor.
    var gState = {
        'updatedAt': "",
        'name': "Bot Name...",
        'desc': "Click to edit the description..."
    };

    // Do we have an anchor already?
    var anchor = document.location.hash;
    if (anchor){
        // If yes, get the app state out of it
        gState = extractFromAnchor(anchor);
        console.log(gState);
    }
    // then initialize the app with it
    initFromState(gState);
    initButtonsInputs();

    function initButtonsInputs(){
        document.querySelectorAll('.custom-edit').forEach(($el) => $el.onclick = clickToEdit);
        document.querySelector('.custom-edit-image').onclick = editImageUrl;
        document.querySelector('.custom-edit-conceptArt').onclick = editConceptUrl;
    }

    function editImageUrl(){
        var $img = document.querySelector('.custom-edit-image'); 
        var response = prompt("Edit the image URL", $img.src);
        response = (response === null)? $img.src : response;
        $img.src = response;
        updateState('image', response);
    }
    function editConceptUrl(){
        var $img = document.querySelector('.custom-edit-conceptArt'); 
        var response = prompt("Edit the concept art image URL", $img.src);
        response = (response === null)? $img.src : response;
        $img.src = response;
        updateState('conceptArt', response);
    }
    function clickToEdit(e){
        var $el = e.target;
        var editedFieldId = getCustomEditId($el);
        var response = prompt("Edit the field: "+editedFieldId, $el.innerText);
        response = (response === null)? $el.innerText : response;
        response = (response.match(/^\s*$/)?.length)? "click to edit..." : response;
        var newFieldValue = response;
        $el.innerText = newFieldValue;
        updateState(editedFieldId, newFieldValue);
    }
    function updateState(id, val){
        gState[id] = val;
        gState['updatedAt'] = new Date().toString();
        document.querySelector('.custom-edit-updatedAt').innerText = gState['updatedAt'];
        exportState();
    }

    function getCustomEditId($el){
        return Array.from($el.classList).filter((className) => className.startsWith('custom-edit-'))[0].slice('custom-edit-'.length)
    }


    function exportState(){
        // we do the reverse than in extractFromAnchor()
        var data = JSON.stringify(gState);
        var encoded = btoa(data);
        var anchor = '#'+encoded;
        // update the anchor
        document.location.hash = anchor;
    }


    function extractFromAnchor(anchor){
        // remove the #
        var data = anchor.slice(1);
        // the data will be base64-encoded to avoid special characters issues
        var decoded = atob(data) 
        // let's assume we serialize the data as json
        return JSON.parse(decoded);
    }


    // paste all the values from the url into the page
    function initFromState(state){
        document.querySelectorAll('.custom-edit').forEach( ($el) => {
            var fieldId = getCustomEditId($el);
            if (fieldId in gState){
                $el.innerText = gState[fieldId];
            }
        })
        if ('image' in gState) document.querySelector('.custom-edit-image').src = gState['image'];
        if ('conceptArt' in gState) document.querySelector('.custom-edit-conceptArt').src = gState['conceptArt'];
    }
</script>

  
