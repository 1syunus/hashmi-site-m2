* {
    box-sizing: border-box;
}

body {
    margin: 0;
    padding: 0;
    display: flex;
    min-height: 100vh;
    }
    
    .container {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        border-radius: 10px;
        overflow: hidden;
        background-color: whitesmoke;
        width: 100vw;
        padding-right: .2em;
    }
    
    
    .content {
        display: flex;
        flex: 2;
        margin-top: 0;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        margin-left: 0;
        padding: 0;
        width: 100vw;
        background-image: url("images/note-med.jpg"), linear-gradient(rgba(245, 245, 245, 0.82),rgba(245, 245, 245, 0.82));
        background-blend-mode: overlay;
        background-position: center;
    }
    
    .logo-front {
        z-index: 2;
        width: 9em;
        height: 9em;
        border-radius: 50%;
        box-shadow: 2px 2px 5px #ccc;

    }

    .doc {
      font-size: 3rem;
      z-index: 1;
      opacity: .5;
      color: gray;
    }

    h1::before {
      content: "Dr.";
      position: absolute;
      font-family: "Lato";
      top: 29%;
      left: 11%;
      z-index: -1;
      font-size: 6rem;
      color: rgba(112, 128, 144, 0.2);
      -webkit-text-stroke: .1px white;
  }

  h1::after {
    content: "";
    position: absolute;
    top: 40%;
    left: 0;
    right: 0;
    height: 2px;
    background-color: azure;
    box-shadow: 0 0 10px rgba(112, 128, 144, 0.2); 
    z-index: -1;
    clip-path: polygon(
        0% 0%, 
        calc(11% - 25px) 0%, 
        calc(11% - 25px) 100%, 
        0% 100%, 
        100% 100%, 
        100% 0%, 
        calc(11% + 110px) 0%, 
        calc(11% + 110px) 100%, 
        0% 100%
    );
}
    
    h1 {
        font-family: "Lato", serif;
        font-size: 2rem;
        letter-spacing: .2em;
        color: #4169E1;
        opacity: .9;
        z-index: 2;
        font-weight: 300;
    }
    
    h1 span {
        font-size: 4rem;
        color: seagreen;
        filter:brightness(1.3);
    
    }
    
    p {
        font-family: "Audiowide", system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        letter-spacing: 1.2em;
        font-size: 1.1rem;
        font-weight: 900;
        color: slategrey;
        text-shadow: 1px 1px 1px azure;
        margin-top: 0;
        padding-top: 0;
        line-height: 1.4;
    }
    
    .contact-btn {
        background-color: transparent;
        font-family: "Montserrat";
        font-weight: 600;
        color: #4169E1;
        font-size: 1rem;
        text-decoration: none;
        text-align: center;
        padding: .5em 5.5em;
        margin: 5em 2em 0 2em;
        border-radius: .3rem;
        border: solid .03rem seagreen;
        transition: all .3s ease;

    }
    
    .contact-btn:hover {
        background-color: rgb(125 219 163);
        color: whitesmoke;        
        border-color: transparent;
        /* opacity: .7; */
    }
    
    .socials {
      margin-top: 4em;  
    }
    
    a .fab {
        text-decoration: none;
    }
      
      ul {
        position: absolute;
        transform: translate(-50%, -50%);
        margin: 0;
        padding: 0;
        display: flex;
      }
      
      ul li {
        list-style: none;
      }
      
      ul li a {
        position: relative;
        width: 45px;
        height: 45px;
        display: block;
        margin: 0 10px;
        border-radius: 50%;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
        text-decoration: none;
      }
      
      ul li a:hover {
        transform: translateY(-5px);
        text-shadow: 0 0 2px;
    
      }
      
      ul li a .fab {
        position: relative;
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 24px;
        color: #262626;
        
      }
      
      ul li:nth-child(1) a:hover .fab {
        color: #3b5998;
      }
      
      ul li:nth-child(2) a:hover .fab {
        color: #00aced;
      }
      
      ul li:nth-child(3) a:hover .fab {
        color: #dd4b39;
      }
      
      ul li:nth-child(4) a:hover .fab {
        color: #007bb6;
      }
      
      ul li:nth-child(5) a:hover .fab {
        color: #e4405f;
      }
      
      @media (min-width: 768px) {
        body {
          justify-content: center;
          align-items: center;
          min-height: 100vh;
          background-color: #f8f9fa
        }
    
        .container {
          flex-direction: row;
          min-height: 100vh;
        }
    
        .img {
          flex: 1;
          background-image: url("images/note-med.jpg"); 
          background-position: center;
          background-repeat: no-repeat;
          background-size: cover;
          opacity: .9;      
        }
    
        .content {
          flex: 1;
          background-color: whitesmoke;
          background-image: none;
        }

        /* h1 {
          margin-left: 3.5em;
        }

        h1::before {
          font-family: "Lato";
          top: 38%;
          left: 51%;
          z-index: 2;
          font-size: 4rem;
          color: rgba(112, 128, 144, 0.4);
          -webkit-text-stroke: .1px white;
      }
        
        h1::after {
          display: none;
        } */
    }
    