<html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Quick Reads</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: #f0f0f0;
    }

    header {
      background: #2e7d32;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .tabs {
      display: flex;
      background: #ddd;
      border-bottom: 2px solid #ccc;
      overflow-x: auto;
    }

    .tab {
      padding: 10px 20px;
      cursor: pointer;
      background: #ccc;
      border-right: 1px solid #bbb;
      white-space: nowrap;
    }

    .tab.active {
      background: white;
      border-bottom: 2px solid white;
      font-weight: bold;
    }

    .tab-content {
      display: none;
      padding: 20px;
      background: white;
    }

    .tab-content.active {
      display: block;
    }

    .story {
      margin-top: 10px;
      line-height: 1.6;
    }

    .rating {
      margin-top: 15px;
    }

    .stars {
      cursor: pointer;
      font-size: 20px;
      color: gray;
    }

    .stars.selected {
      color: gold;
    }

    .comments-section {
      margin-top: 20px;
    }

    .comment-form input {
      margin-bottom: 10px;
    }

    @media (max-width: 600px) {
      .tab {
        padding: 10px;
        font-size: 14px;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>📖 Quick Reads</h1>
    <p>Short Stories. Big Impact.</p>
  </header>

  <div class="tabs">
    <div class="tab active" data-tab="home">🏠 Home</div>
    <div class="tab" data-tab="story-1">🌲 Forest</div>
    <div class="tab" data-tab="story-2">🤖 Robot</div>
    <div class="tab" data-tab="trailers">🎬 Trailers</div>
  </div>

  <!-- Home Tab -->
  <div id="home" class="tab-content active">
    <h2>About Quick Reads</h2>
    <p>
      Welcome to <strong>Quick Reads</strong> — your space for engaging, bite-sized stories you can enjoy anytime, anywhere.
      <br><br>
      ✅ No sign-ups. <br>
      ✅ No distractions. <br>
      ✅ Just quick, memorable stories.
    </p>
    <p>
      Use the tabs above to explore different stories. Rate them, leave a comment, and enjoy reading like you're browsing tabs in Chrome.
    </p>
  </div>

  <!-- Story 1 -->
  <div id="story-1" class="tab-content">
    <h2>The Murder Files Of 2008</h2>
    <div class="story">
      A scream, a thud, police sirens going their usual rythmaic tone of 'Wee Woo', and the annoying noise of repoters asking the same questions a hundred time, not to mention that police sirens were equally annoying too. These were the sound that the residents near the house of the Mayor of the city Cloville, Mrs. Kathleen Crest, heard at the dusk of dawn, around 6, on the dreadful date of 17th October, 2008. And if it wasn't obvious enough, these events took place, because Mrs. Kathleen had fell two stories, and died.
    </div>

    <div class="rating" data-story="story-1">
      <strong>Rate this story:</strong><br>
      <span class="stars" data-value="1">&#9733;</span>
      <span class="stars" data-value="2">&#9733;</span>
      <span class="stars" data-value="3">&#9733;</span>
      <span class="stars" data-value="4">&#9733;</span>
      <span class="stars" data-value="5">&#9733;</span>
    </div>

    <hr>

    <div class="comments-section" data-story="story-1">
      <h3>💬 Comments</h3>
      <form class="comment-form">
        <input type="text" placeholder="Your name" required class="name-input" style="width: 45%; padding: 6px;" />
        <input type="text" placeholder="Write a comment..." required class="comment-input" style="width: 45%; padding: 6px;" />
        <button type="submit" style="padding: 6px 12px;">Post</button>
      </form>
      <ul class="comment-list" style="list-style: none; padding: 0; margin-top: 10px;"></ul>
    </div>
  </div>

  <!-- Story 2 -->
  <div id="story-2" class="tab-content">
    <h2>Robot in the Rain</h2>
    <div class="story">
      Z3X was not built to feel emotion, yet the falling rain sparked a memory he didn’t have...
    </div>

    <div class="rating" data-story="story-2">
      <strong>Rate this story:</strong><br>
      <span class="stars" data-value="1">&#9733;</span>
      <span class="stars" data-value="2">&#9733;</span>
      <span class="stars" data-value="3">&#9733;</span>
      <span class="stars" data-value="4">&#9733;</span>
      <span class="stars" data-value="5">&#9733;</span>
    </div>

    <hr>

    <div class="comments-section" data-story="story-2">
      <h3>💬 Comments</h3>
      <form class="comment-form">
        <input type="text" placeholder="Your name" required class="name-input" style="width: 45%; padding: 6px;" />
        <input type="text" placeholder="Write a comment..." required class="comment-input" style="width: 45%; padding: 6px;" />
        <button type="submit" style="padding: 6px 12px;">Post</button>
      </form>
      <ul class="comment-list" style="list-style: none; padding: 0; margin-top: 10px;"></ul>
    </div>
  </div>

  <!-- Trailers -->
  <div id="trailers" class="tab-content">
    <h2>🎬 Upcoming Stories – Trailers</h2>
    
    <div style="margin-bottom: 30px;">
      <h3>🕯️ Whispers in the Attic</h3>
      <iframe width="100%" height="315" src="https://www.youtube.com/embed/YOUTUBE_VIDEO_ID" 
        title="Whispers in the Attic Trailer" frameborder="0" allowfullscreen></iframe>
      <p>A psychological horror tale about a boy who hears strange voices coming from a locked attic...</p>
    </div>

    <div style="margin-bottom: 30px;">
      <h3>🌌 Across the Void</h3>
      <video width="100%" height="315" controls>
        <source src="teaser-across-the-void.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <p>A space traveler trapped in a time loop tries to send one final message home.</p>
    </div>
  </div>

  <!-- JavaScript -->
  <script>
    // Tabs
    const tabs = document.querySelectorAll('.tab');
    const contents = document.querySelectorAll('.tab-content');

    tabs.forEach(tab => {
      tab.addEventListener('click', () => {
        tabs.forEach(t => t.classList.remove('active'));
        tab.classList.add('active');

        const target = tab.getAttribute('data-tab');
        contents.forEach(c => {
          c.classList.remove('active');
          if (c.id === target) c.classList.add('active');
        });
      });
    });

    // Ratings
    document.querySelectorAll('.rating').forEach(ratingDiv => {
      const storyId = ratingDiv.dataset.story;
      const saved = localStorage.getItem("rating_" + storyId);
      if (saved) highlightStars(ratingDiv, parseInt(saved));
    });

    document.querySelectorAll('.stars').forEach(star => {
      star.addEventListener('click', () => {
        const value = parseInt(star.dataset.value);
        const ratingDiv = star.closest('.rating');
        const storyId = ratingDiv.dataset.story;
        localStorage.setItem("rating_" + storyId, value);
        highlightStars(ratingDiv, value);
      });
    });

    function highlightStars(ratingDiv, rating) {
      const stars = ratingDiv.querySelectorAll('.stars');
      stars.forEach(s => {
        const val = parseInt(s.dataset.value);
        s.classList.toggle('selected', val <= rating);
      });
    }

    // Comments
    document.querySelectorAll('.comments-section').forEach(section => {
      const storyId = section.dataset.story;
      const form = section.querySelector('.comment-form');
      const nameInput = section.querySelector('.name-input');
      const commentInput = section.querySelector('.comment-input');
      const commentList = section.querySelector('.comment-list');

      const savedComments = JSON.parse(localStorage.getItem("comments_" + storyId)) || [];
      savedComments.forEach(c => addCommentToList(commentList, c.name, c.text));

      form.addEventListener('submit', e => {
        e.preventDefault();
        const name = nameInput.value.trim();
        const comment = commentInput.value.trim();
        if (name && comment) {
          addCommentToList(commentList, name, comment);
          savedComments.push({ name, text: comment });
          localStorage.setItem("comments_" + storyId, JSON.stringify(savedComments));
          nameInput.value = '';
          commentInput.value = '';
        }
      });
    });

    function addCommentToList(list, name, text) {
      const li = document.createElement('li');
      li.style.borderBottom = "1px solid #ccc";
      li.style.padding = "6px 0";
      li.innerHTML = `<strong>${name}:</strong> ${text}`;
      list.appendChild(li);
    }
  </script>

</body>
</html>
