<script>
  import { onMount } from 'svelte';
  import "./home.css";

  let video;

  onMount(() => {
      if (video) {
          video.muted = true;
          video.play();
      }
  });

  const toggleSound = () => {
      if (video) {
          video.muted = !video.muted;
          adjustAudioDisabledSymbol();
      }
  };

  const adjustAudioDisabledSymbol = () => {
      if (video.muted) {
          document.getElementById("audio-disabled").classList.add("audio-disabled");
      } else {
          document.getElementById("audio-disabled").classList.remove("audio-disabled");
      }
  };
</script>

<div class="home">
  <div class="video-container">
      <a href="https://www.youtube.com/watch?v=7uHk07dQGO0" target="_blank" aria-label="YouTube - Syracouse Affair teaser">
          <video bind:this={video} autoplay loop muted playsinline>
              <source src="/video/video.mp4" type="video/mp4">
          </video>
      </a>
      <button class="audio-control" aria-label="toggle sound" on:click={toggleSound}>
          <div class="audio-disabled-marker audio-disabled" id="audio-disabled"></div>
      </button>
  </div>
</div>
