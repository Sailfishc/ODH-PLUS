<template>
  <div class='container'>
        <form>
            <div class="grouppanel">
                <div class="grouptitle">
                    <span class="title" data-i18n="baTitle">Options</span>
                    <span class="more" id="more">...</span>
                </div>
                <div class="crosspanel">
                    <label data-i18n="baEnabled">Enabled</label>
                    <div class="enabled">
                        <input type="checkbox" value=true id="enabled">
                        <label for="enabled"></label>
                    </div>
    
                    <label data-i18n="baHotKey">AuoSel.</label>
                    <select id="hotkey">
                        <option value="0">Off</option>
                        <option value="16">Shift</option>
                        <option value="17">Ctrl</option>
                        <option value="18">Alt</option>
                    </select>
                    <hr class="anki-options">
                    <select id="deckname" class="anki-options col-2x">
                        <option value=""></option>
                    </select>
                    <hr>
                    <select id="dict" class="col-2x">
                        <option value="encn-Default">encn-Default</option>
                    </select>
                </div>
            </div>
        </form>
    </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style scoped>
.container {
    margin: 0;
    padding: 0;
}
.grouppanel {
    border-radius: 5px;
    background-color: #f1f8e9;
    margin: 5px 0;
    padding: 0 0 3px;
}
.grouptitle {
    font-weight: bold;
    color: white;
    background-color: #93a085;
    border-radius: 5px 5px 0 0;
    margin: 0 0 4px;
    padding: 4px 15px;
}

.crosspanel {
    padding: 0 6px;
    width: 100%;
}

a {
    text-decoration: none;
}

.more {
    float: right;
    color: white;
    cursor: pointer;
}

label,
select {
    width: 95px;
    padding: 4px 5px;
    margin: 3px;
    display: inline-block;
    color: black;
    border: 1px solid #d5d5d5;
    border-radius: 4px;
}

label {
    border-style: dashed;
}

.col-2x {
    width: 200px;
}

hr {
    border: 1px;
    margin: 4px 5px;
    border-top: 1px solid #e5e5e5;
}

.enabled input[type=checkbox] {
    visibility: hidden;
}

.enabled {
    width: 65px;
    height: 26px;
    display:inline-block;
    background: #555;
    margin: 3px;
    border-radius: 25px;
    top:-2px;
    position: relative;
}

.enabled:before {
    content: 'On';
    position: absolute;
    top: 5px;
    left: 10px;
    height: 1px;
    color: #76ff03;
    font-weight: bold;
}

.enabled:after {
    content: 'Off';
    position: absolute;
    top: 5px;
    left: 35px;
    height: 1px;
    color: #f9f9f9;
    font-weight: bold;
}

.enabled label {
    display: block;
    width: 26px;
    height: 16px;
    border: none;
    border-radius: 37px;
    transition: all .5s ease;
    cursor: pointer;
    position: absolute;
    top: 2px;
    z-index: 1;
    left: 4px;
    background: #ddd;
}

.enabled input[type=checkbox]:checked+label {
    left: 28px;
    background: #76ff03;
}
</style>
