<style>
    .card {
      perspective: 500px;
    }
  
    .content {
      display: flex;
      align-items: center;
      justify-content: center;
  
    }
  
    .front {
        display: flex;
        flex-direction: column;
        height: 300px;
        width: 200px;
        background-color: rgba(255, 250, 220, 1);
        background-image: url($lib/tess-loteria.svg);
        backface-visibility: hidden;
        border-radius: 10px;
        transition: transform 0.8s; 
        position: absolute;
        align-self: center;
        box-shadow: 0 0 15px rgba(0,0,0,.1);
    }

    .back {
        display: flex;
        flex-direction: column;
        height: 300px;
        width: 200px;
        background-color: rgba(255, 250, 220, 1);
        background-image: url($lib/tess-loteria-2.svg);
        backface-visibility: hidden;
        border-radius: 10px;
        transition: transform 0.8s; 
        position: absolute;
        align-self: center;
        box-shadow: 0 0 15px rgba(0,0,0,.1);

    }
  
    .back {
      transform: rotateY(180deg);
    }
  
    h1 {
        font-family: 'Inter', sans-serif;
      font-weight: 300;
      margin: 0;
      font-size: 2rem;
    }
  
    h2 {
        font-family: 'Inter', sans-serif;
      font-weight: 500;
      margin: 0;
      font-size: 1.5rem;
    }
  
    h3 {
        font-family: 'Inter', sans-serif;
      font-weight: 100;
      margin: 0;
      font-size: 1rem;
    }
  
    .card:hover .front {
      transform: rotateY(180deg);
      cursor: alias;
    }
  
    .card:hover .back {
      transform: rotateY(0);
      cursor: alias;
  
    }
  
    .front-align {
      margin-top: 10%;
      margin-left: 10%;
    }
  

  
  </style>
  

    
      <div class="card">
        <div class="content">
  
  
          <div class="front">
            <div class="front-align">
            </div>
          </div>
  
          <div class="back">

          </div>
          
        </div>
      </div>
    