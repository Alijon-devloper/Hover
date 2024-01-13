@import url("https://fonts.googleapis.com/css2?family=Basic&family=Poppins&display=swap");

:root {
  --background: #000000;
  --background-border: #00fffc;
}
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: Poppins;
    height: 100vh;
    padding: 32px;
    display: grid;
    place-items: center;
    background-color: var(--background);
  }
  
  .gallery {
    display: flex;
    background-color:
     var(--background);
    gap: 16px;
    scale: 1.6;
  }
  
  .card {
    position: relative;
    left: 0px;
    width: 140px;
    height: 160px;
    background-color: var(--background);
    border-radius: 8px;
    transition: 1000ms all;
    transform-origin: center left;
    box-shadow: 0 5px 12px rgba(0, 0, 0, 0.5);
    outline: 1px solid var(--background);
    overflow: hidden;
  }
  
  .card img {
    height: 160px;
    object-fit: cover;
    border-radius: 4px;
  }
  .card:hover {
    cursor: pointer;
    transform: scale(1.15);
    box-shadow: 0 0 20px
     #00fffc;
    margin: 5px;
  }
  .card:hover figcaption {
    font-size: 0.6rem;
    position: absolute;
    height: 80px;
    width: 160px;
    display: flex;
    align-items: end;
    background: linear-gradient(
      to top,
      rgba(0, 0, 0, 0.9) 0%,
      rgba(0, 0, 0, 0) 100%
    );
    color: white;
    left: 0px;
    bottom: 0px;
    padding-left: 12px;
    padding-bottom: 10px;
  }
  
  .card:hover ~ .card {
    font-weight: bold;
    cursor: pointer;
    transform: translateX(22px);
  }
  
  
  
  /* -- YouTube Link Styles -- */
  
  #source-link {
    top: 60px;
  }
  
  #source-link > i {
    color: rgb(94, 106, 210);
  }
  
  #yt-link {  
    top: 10px;
  }
  
  #yt-link > i {
    color: rgb(219, 31, 106); 
  
  }
  
  .meta-link {
    align-items: center;
    backdrop-filter: blur(3px);
    background-color: rgba(255, 255, 255, 0.05);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 6px;
    box-shadow: 2px 2px 2px rgba(0, 0, 0, 0.1);
    cursor: pointer;  
    display: inline-flex;
    gap: 5px;
    left: 10px;
    padding: 10px 20px;
    position: fixed;
    text-decoration: none;
    transition: background-color 600ms, border-color 600ms;
    z-index: 10000;
  }
  
  .meta-link:hover {
    background-color: rgba(255, 255, 255, 0.1);
    border: 1px solid rgba(255, 255, 255, 0.2);
  }
  
  .meta-link > i, .meta-link > span {
    height: 20px;
    line-height: 20px;
  }
  
  .meta-link > span {
    color: white;
    font-family: "Rubik", sans-serif;
    transition: color 600ms;
  }
  
