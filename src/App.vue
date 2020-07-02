<template>
  <div id="app">
    <div class="content">{{ word }}</div>
    <button @click="clicked">תלחצייי על זההה</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      array: [
        "איש",
        "‎הר",
        "‎מדינה",
        "‎אוקינוס",
        "‎מחוז",
        "‎בניין",
        "‎חתול",
        "‎חברת תעופה",
        "‎אהב",
        "‎עושר",
        "‎אושר",
        "‎גאווה",
        "‎פחד",
        "‎דת",
        "‎אמונה",
        "היסטוריה",
        "‎תקשורת",
        "‎בית",
        "‎אוקיינוס",
        "‎הדוד מייק",
        "‎ציפור",
        "‎צילום",
        "‎בננה",
        "‎עיניים",
        "אור",
        "‎שמש",
        "‎כלב",
        "‎מזוודה",
        "‎פרחים",
        "‎מיטה",
        "‎חתול",
        "‎סרט",
        "‎רכבת",
        "‎מדינה",
        "‎ספר",
        "‎טלפון",
        "‎משחק",
        "‎רמקול",
        "‎שעון‎עט",
        "‎כינור",
        "חלב",
        "‎אוכל",
        "‎מוזיקה",
        "‎מפה",
        "‎משקפיים",
        "‎ניו יורק",
        "‎תמונה",
        "‎כלה",
        "‎צמות",
        "‎אור שמש",
        "בובספוג",
        "סופר מן",
        "ראש העיר",
        "ראש הממשלה",
        "כוכב",
        "חללית",
        "קרמבולה"
      ],
      word: "loading"
    };
  },
  created() {
    this.word = this.array[Math.floor(Math.random() * this.array.length)];
  },
  methods: {
    clicked() {
      this.word = this.array[Math.floor(Math.random() * this.array.length)];
    }
  }
};
</script>

<style>
body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #dae1e7;
  background-color: #142850;
}

button {
  margin-top: 1rem;
  background-color: #00909e; /* Green */
  border: none;
  color: white;
  padding: 15px 26px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}

.content {
  margin-top: 5rem;
  font-size: 3rem;
}
</style>
