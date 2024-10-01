<gridLayout rows="auto, auto, auto, *, *" columns="auto, *, *" class="profile-grid">

  <image src="~/assets/profile.png" row="0" col="0" class="profile-picture" />

  <gridLayout row="0" col="1" colSpan="2" rows="auto, auto, auto, auto" columns="*" class="user-info">
    <label text="Jirka Miklusčák" class="user-name" font-family="'Archabeta Bold', 'archabeta-bold'" fontWeight="700"/>
    <label textWrap="true" text="Milovník divadla, především klasických tragédií." row="1" col="0" class="bio" font-family="'Archabeta Regular', 'archabeta-regular'" fontWeight="300"/>
    <label text="#romeoajulie #shakespear" row="2" col="0" class="hashtags" font-family="'Archabeta Bold', 'archabeta-bold'" fontWeight="700"/>
    <label text="🌐" row="3" col="0" class="social-media" />
  </gridLayout>

  <label text="Poslední navštívené hry" row="3" col="0" colSpan="3" class="watched-movies"/>

  <label text="Komentáře" row="4" col="0" colSpan="3" class="comments" />
  
</gridLayout>

<style>

  .profile-grid {
    gap: 20px;
    background-color: #f0f0f0;
    padding: 20px;
    height: 100vh; 
  }

  .profile-picture {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    object-fit: cover;
    margin: 10;
  }

  .user-info {
    padding: 10px;
    margin-left: 50px;
    margin-top: 30px;
  }

  .user-name {
    font-size: 22px;
    color: #0f0f0f;
    padding: 5px;
    border-radius: 5px;
  }

  .bio {
    font-size: 16px;
    color: #0f0f0f;
    margin-top: 10px;
  }

  .hashtags {
    font-size: 16px;
    color: #3c3c3c;
    margin-top: 10px;
  }

  .watched-movies {
    background-color: #f0f0f0;
    color: #0f0f0f;
    padding: 10px;
    text-align: center;
    border-radius: 10%;
    width: 100%;
    height: 38%;
    border-width: 8;
    border-color: #ff4c00;
    font-family: 'Archabeta ExtraBold', 'archabeta-extrabold';
    font-weight: 800;
  }

  .comments {
    background-color: #f0f0f0;
    color: #0f0f0f;
    padding: 10px;
    text-align: center;
    border-radius: 10%;
    width: 100%;
    height: 38%;
    border-width: 8;
    border-color: #64d13e;
    font-family: 'Archabeta ExtraBold', 'archabeta-extrabold';
    font-weight: 800;
    margin-top: 5;
  }

  .profile-grid > .watched-movies, .profile-grid > .comments {
    flex: 1;
  }

  .social-media {
    text-align: right;
  }
</style>
