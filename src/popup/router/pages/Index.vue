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

<style lang="less" scoped>
    
</style>
