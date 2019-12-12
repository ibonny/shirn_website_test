 <template>
    <div class="container">
        <div>
            <input type="text" v-model="text" /><br/>
            <br/>
            <span class="shirn">{{ text }}</span><br/>
            <span class="dardanian">{{ text }}</span><br/>
            <span class="nirichaen">{{ text }}</span><br/>
            <span class="tengwar">{{ text }}</span><br/>
            <span class="enganagri">{{ text }}</span>
        </div>
    </div>
</template>

<script>
export default {
    "data": function() {
        return {
            "text": ""
        }
    },
    "head": function() {
        return {
            "title": "Various font tests"
        }
    }
}
</script>

<style>
body {
    margin-top: 20px;
    margin-left: 20px;
}

@font-face {
    font-family: 'shirn';
    src: url("/shirn_website_test/shirn.otf")
}

@font-face {
    font-family: 'dardanian';
    src: url("/shirn_website_test/dardanian.ttf");
}

@font-face {
    font-family: 'nirichaen';
    src: url('/shirn_website_test/nirichaen.ttf');
}

@font-face {
    font-family: "tengwar";
    src: url("/shirn_website_test/tngani.ttf");
}

@font-face {
    font-family: "/enganigri";
    src: url("/shirn_website_test/Enganagri.ttf")
}

.shirn {
    font-family: "shirn", "Georgia", serif;
    font-size: 30px;
}

.dardanian {
    font-family: "dardanian", "Georgia", serif;
    font-size: 30px;
}

.nirichaen {
    font-family: "nirichaen", "Georgia", serif;
    font-size: 30px;
}

.tengwar {
    font-family: "tengwar", "Georgia", serif;
    font-size: 30px;
}

.enganagri {
    font-family: "enganagri", "Georgia", serif;
    font-size: 30px;
}
</style>
