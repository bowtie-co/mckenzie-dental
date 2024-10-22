---
location: 'homepage'
head:
  pretitle:
  title:
  subtitle: null


style:
  id: ''
  class: 'contained text-center test'
  media:
    img_path:
      url_path:
      pattern: false
      parallax: false
      overlay: light
      blur: false
    video:
      url_path:
      type:
    slides:

  tint_color: null
  font_color: '#000'
published: true
---


<!-- <iframe src="https://player.vimeo.com/video/448564581" width="100%" height="auto" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe> -->

<style>
  .video-container {
    position: relative;
    width: 100%;
    max-width: 1200px; /* Set your preferred max width */
    padding-bottom: 56.25%; /* 16:9 aspect ratio */
    height: 0;
    margin: 0 auto; /* Center the container horizontally */
  }

  .video-iframe, .video-poster {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
  }

  .video-iframe {
    display: none; /* Initially hide the iframe */
  }

  .video-poster {
    background-image: url('master_hero_images/mckenzie-heroes/McKenzieDental-thumb.jpg');
    background-size: cover;
    background-position: center;
    cursor: pointer;
    z-index: 2; /* Keep it on top until clicked */
  }
</style>
<!-- <div class='embed-container'><iframe src='https://www.youtube.com/embed/YyXt36Njuoo' frameborder='0' webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe></div> -->


<div class="video-container">
  <!-- Poster image -->
  <div class="video-poster" id="videoPoster"></div>

  <!-- YouTube iframe, initially hidden -->
  <iframe id="youtubeIframe" class="video-iframe"
    src="https://www.youtube.com/embed/YyXt36Njuoo?enablejsapi=1"
    frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<script>
  // When the poster is clicked, hide the poster and load the YouTube video
  document.getElementById('videoPoster').addEventListener('click', function() {
    // Hide the poster
    this.style.display = 'none';

    // Show the iframe and add the autoplay parameter to start the video
    const iframe = document.getElementById('youtubeIframe');
    iframe.src += "&autoplay=1&modestbranding=1&showinfo=0";
    iframe.style.display = 'block';
  });
</script>
<!-- <p><a href="https://vimeo.com/448564581">McKenzie Dental COVID Safety Video</a> from <a href="https://vimeo.com/user121549023">Robert Kelly</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

<h4>At McKenzie Dental we are doing everything we can to keep you and the community safe.  Click here for a video on some of our safety procedures.</h4>
<br /> -->
