<script>
  export let width;
  export let height;
  export let image;
  export let imageSize;
  export let name;
  export let rotation;
</script>

<div class="portrait-background" style:width={width} style:height={height} style:transform={`rotate(${rotation}deg)`}>
  <div class="portrait-image" style:background-image={image} style:width={imageSize} style:height={imageSize}></div>
  <div class="portrait-text">{name}</div>
</div>

<style>
  .portrait-background {
    background-color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .portrait-image {
    background-color: #fff;
    margin: 0 auto 10px auto;
  }

  .portrait-text {
    font-family: "FuzzyBubbles";
    color: #000;
    font-size: 24px;
    text-align: center;
    margin: 0 auto;
  }
</style>