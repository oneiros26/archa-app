<gridLayout rows="auto, auto, auto, *, *" columns="auto, *, *" class="profile-grid">
  <!-- Profile Picture (Image) -->
  <image src="~/assets/profile.png" row="0" col="0" class="profile-picture" />

  <!-- User Info Section (User Name, Bio, Hashtags, Socials) -->
  <gridLayout row="0" col="1" colSpan="2" rows="auto, auto, auto, auto" columns="*" class="user-info">
    <label text="Uživatel" class="user-name" />
    <label text="Bio/popisek" row="1" col="0" class="bio" />
    <label text="#hashtag1 #hashtag2" row="2" col="0" class="hashtags" />
    <label text="🌐" row="3" col="0" class="social-media" />
  </gridLayout>

  <!-- Watched Movies Section (Full width, below profile picture and user info) -->
  <label text="Sledované" row="3" col="0" colSpan="3" class="watched-movies" />

  <!-- Comments Section (Full width, below Watched Movies) -->
  <label text="Komentáře" row="4" col="0" colSpan="3" class="comments" />
</gridLayout>

<style>
  /* Overall Grid Layout */
  .profile-grid {
    gap: 20px;
    background-color: #000;
    padding: 20px;
    height: 100vh; /* Full viewport height */
  }

  /* Profile Picture: Grid Item */
  .profile-picture {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    object-fit: cover;
    background-color: #1a1a1a;
  }

  /* User Info Section */
  .user-info {
    padding: 10px;
    margin-left: 50px;
    margin-top: 30px;
  }

  .user-name {
    font-size: 20px;
    color: #fff;
    padding: 5px;
    border-radius: 5px;
  }

  .bio {
    font-size: 14px;
    color: #fff;
    margin-top: 10px;
  }

  .hashtags {
    font-size: 12px;
    color: #aaa;
    margin-top: 10px;
  }

  /* Watched Movies */
  .watched-movies {
    background-color: #333;
    color: white;
    padding: 10px;
    text-align: center;
    border-radius: 10px;
    width: 100%; /* Full width */
    height: 100%; /* Takes remaining available space */
  }

  /* Comments */
  .comments {
    background-color: #555;
    color: white;
    padding: 10px;
    text-align: center;
    border-radius: 10px;
    width: 100%; /* Full width */
    height: 100%; /* Takes remaining available space */
  }

  /* Ensure the watched movies and comments fill the screen */
  .profile-grid > .watched-movies, .profile-grid > .comments {
    flex: 1;
  }

  .social-media {
    text-align: right;
  }
</style>
