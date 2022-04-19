<template>
  <div class="articles">
    <div class="card" style="--cards:5">
      <div class="child">
        <h2>Why do I need a will</h2>
        <p>5 articles</p>
      </div>
      <div class="child"></div>
      <div class="child"></div>
      <div class="child"></div>
      <div class="child"></div>
    </div>
    <div class="card" style="--cards:3">
      <div class="child">
        <h2>How to choose who inherits your estate</h2>
        <p>3 articles</p>
      </div>
      <div class="child"></div>
      <div class="child"></div>
    </div>
    <div class="card" style="--cards:2">
      <div class="child">
        <h2>What happens when you die</h2>
        <p>2 articles</p>
      </div>
      <div class="child"></div>
    </div>
    <div class="card" style="--cards:4">
      <div class="child">
        <h2>How to choose guardians</h2>
        <p>4 articles</p>
      </div>
      <div class="child"></div>
      <div class="child"></div>
      <div class="child"></div>
    </div>
    <div class="card" style="--cards:4">
      <div class="child">
        <h2>Why you've been disinherited</h2>
        <p>4 articles</p>
      </div>
      <div class="child"></div>
      <div class="child"></div>
      <div class="child"></div>
    </div>
    <div class="card" style="--cards:3">
      <div class="child">
        <h2>How to commit fraud, legally</h2>
        <p>3 articles</p>
      </div>
      <div class="child"></div>
      <div class="child"></div>
    </div>
    <div class="card" style="--cards:5">
      <div class="child">
        <h2>Stay together for the kids</h2>
        <p>5 articles</p>
      </div>
      <div class="child"></div>
      <div class="child"></div>
      <div class="child"></div>
    </div>
    <div class="card" style="--cards:3">
      <div class="child">
        <h2>Picking music for your funeral</h2>
        <p>3 articles</p>
      </div>
      <div class="child"></div>
      <div class="child"></div>
    </div>
  </div>
</template>

<style scoped>
    .articles {
      overflow: auto;
      border: 5px solid lightblue;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
      grid-gap: 48px;
      margin: 0 auto;
    }

  body {
    background: #F9F9F9;
    color: #495456;
    margin: 72px;
    font-family: Open Sans, sans-serif;
  }

  h2 {
    font-family: Arbutus Slab, serif;
    font-weight: normal;
    color: #000;
    line-height: 1.25;
  }

  p {
    position: absolute;
    bottom: 0;
    font-size: 14px;
  }

  .card {
    cursor: pointer;
    position: relative;
    height: 0;
    padding-bottom: 120%;
    --offset-multiplier: 4px;
    transition: transform 0.6s ease;
    --translate: 0;
    transform: translate(var(--translate), var(--translate));
  }
  .card:hover {
    --offset-multiplier: 6px;
  }
  .card:hover {
    --translate: calc(-1px * (var(--cards) - 1));
    transition: transform 0.3s ease;
  }

  .child {
    position: absolute;
    width: 100%;
    height: 100%;
    padding: 0 16px;
    box-sizing: border-box;
    background: #fff;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1), 0px -4px 8px rgba(255, 255, 255, 0.8);
    border-radius: 6px;
    transition: inherit;
    --translate: calc(var(--offset) * var(--offset-multiplier));
    transform: translate(var(--translate), var(--translate));
    z-index: 5;
  }
  .child:nth-child(1) {
    --offset: 0;
    z-index: 4;
  }
  .child:nth-child(2) {
    --offset: 1;
    z-index: 3;
  }
  .child:nth-child(3) {
    --offset: 2;
    z-index: 2;
  }
  .child:nth-child(4) {
    --offset: 3;
    z-index: 1;
  }
  .child:nth-child(5) {
    --offset: 4;
    z-index: 0;
  }
</style>
