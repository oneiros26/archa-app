<gridLayout rows="auto, auto, auto, *, auto" columns="auto, *, *" class="profile-grid">
  <!-- Profile Picture (Image) -->
  <image src="~/assets/profile.png" row="0" col="0"  class="profile-picture" />

  <!-- User Info Section (User Name, Bio, Hashtags, Socials) -->
  <gridLayout row="0" col="1" colSpan="2" rows="auto, auto, auto, auto" columns="*" class="user-info">
    <label text="Uživatel" class="user-name" />
    <label text="Bio/popisek" row="1" col="0" class="bio" />
    <label text="#hashtag1 #hashtag2" row="2" col="0" class="hashtags" />
    <label text="🌐" row="3" col="0" class="social-media" />
  </gridLayout>

  <!-- Comments Section -->
  <label text="Komentáře" row="2" col="0" rowSpan="2" class="comments" /> <!-- Moved down to prevent overlap -->

  <!-- Watched Movies Section -->
  <label text="Sledované" row="2" col="1" colSpan="2" class="watched-movies" /> <!-- Adjusted position -->
</gridLayout>

<style>
  /* Overall Grid Layout */
  .profile-grid {
    gap: 20px;
    background-color: #000;
    padding: 20px;
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
  }

  .user-name {
    font-size: 20px;
    color: #fff;
    /*background-color: #64d13e;*/
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

  /* Comments */
  .comments {
    background-color: #555;
    color: white;
    padding: 10px;
    text-align: left;
    margin-top: 50px;
    border-radius: 10px; /* Added border radius */
    rowSpan: 2; /* Ensures it spans two rows */
  }

  /* Social Media */
  .social-media {
    background-color: none; /* Added a background color */
    color: white;
    padding: 10px; /* Added padding for aesthetics */
    margin-top: 20px; /* Added margin to create space */
    text-align: right;
  }

  /* Watched Movies */
  .watched-movies {
    color: white;
    text-align: center;
    margin-top: 20px; /* Consistent spacing */
  }
</style>
