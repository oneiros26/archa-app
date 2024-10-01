<gridLayout rows="auto, auto, auto, *, auto" columns="auto, *, *" class="profile-grid">

  <gridLayout row="0" col="1" colSpan="2" rows="auto, auto, auto, auto" columns="*,*" class="user-info">
    <image src="~/assets/profile.png" row="0" col="0"  class="profile-picture" />
    <label text="Alexandr Novák" class="user-name" fontFamily="'Archabeta Bold', 'archabeta-bold'" fontWeight="700"/>
    <label textWrap="true" text="Milovník divadla, který rád objevuje nové inscenace a sdílí zážitky z kulturních představení." row="1" col="0" class="bio" fontFamily="'Archabeta Regular', 'archabeta-regular'" fontWeight="400"/>
    <label text="#romeoajulio #shakespeare" row="2" col="0" class="hashtags" fontFamily="'Archabeta Bold', 'archabeta-bold'" fontWeight="700"/>
    <label text="" row="3" col="0" class="social-media" fontFamily="'Font Awesome 5 Free', 'fa-regular-400'"/>
  </gridLayout>

  <gridLayout row="1" col="0" colSpan="3" rows="auto, auto" columns="*" class="user-info">
    <label text="Sledované" row="0" col="0" colSpan="2" class="watched-movies" fontFamily="'Archabeta Bold', 'archabeta-bold'" fontWeight="700"/>
    <label text="Komentáře" row="1" col="0" rowSpan="2" class="comments" fontFamily="'Archabeta Bold', 'archabeta-bold'" fontWeight="700"/>
  </gridLayout> 

  
</gridLayout>

<style>

  .profile-grid {
    gap: 20px;
    background-color: #000;
    padding: 20px;
  }

  .profile-picture {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    object-fit: cover;
  }

  .user-info {
    padding: 10px;
    margin-left: 50px;
    margin-top: 80px;
  }

  .user-name {
    font-size: 20px;
    color: #fff;
    padding: 5px;
    border-radius: 5px;
  }

  .bio {
    font-size: 12px;
    color: #fff;
    margin-top: 10px;
  }

  .hashtags {
    font-size: 14px;
    color: #aaa;
    margin-top: 10px;
  }

  .comments {
    background-color: #555;
    color: white;
    padding: 10px;
    text-align: left;
    margin-top: 50px;
    border-radius: 10px;
  }

  .social-media {
    color: #f0f0f0;
    padding: 10px;
    margin-top: 20px; 
    text-align: right;
  }

  .watched-movies {
    color: #f0f0f0;
    text-align: center;
    margin-top: 20px;
  }
</style>
