
html:------------

   <!--prelodder-->

    <div class="ring_loader">
      <div class="ring"></div>
  </div>
  <!--prelodder--> 
  
  css:------------
  
  /*===-prelodder===*/


      .ring_loader{
        width: 100%;
        height: 100vh;
        background-color: #000;
        position: fixed;
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 99999;
      }

      .ring{
        width: 100px;
        height: 100px;
        border: 5px solid;
        color:  #f1c40f;
        border-radius: 50%;
        border-top-color: transparent;
        animation: loader 1.2s linear infinite;
      }

      @keyframes loader{
        10%{
            color: #2ecc71;
        }
        30%{
            color: #f1c40f;
        }
        50%{
            color: #e74c3c;
        }
        75%{
            color:  #f1c40f;
        }
        85%{
            color: #f1c40f;
        }


        to{
            transform: rotate(360deg);
        }
      }
      
        
  
  
  
    //preloader js
      $(window).on("load", function () {
        $(".ring_loader").fadeOut(4000);
      });
      
      
