<!DOCTYPE html>

<html lang="en" >
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta charset="UTF-8">
  <title>Thank you card</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css">
  <link rel="stylesheet" href="./style.css">
  <style type="text/css">
    @import url(https://fonts.googleapis.com/css?family=Open+Sans+Condensed:700);
      *, *:before, *:after {  box-sizing: border-box; }
    html { 
      background: pink;
      height: 100%; 
      width: 100%; }

    body { 
      height: 100%; 
      width: 100%; 
      overflow:hidden;}

    #envelope{
    margin: 100px auto 0;
    position: relative;
    width: 0;
    height: 0;
    z-index: 0;
    border-style: solid;
    border-width: 0 150px 100px 150px;
    border-color: transparent transparent #256a98 transparent;
    box-shadow: 0 100px 0 0 #256a98,
              0 150px 90px 0 rgba(0,0,0,0.3);
}

#envelope:after,
#envelope:before{
  content:'';
  display: block;
  position: absolute;
  top: 100px;
  border-style: solid;
}

#envelope:after{
  width: 0;
  height: 0;
  left: 0;
  border-width: 100px 150px 100px 0;
  border-color: transparent #2a7fb5 transparent transparent;
}

#envelope:before{
  width: 210px;
  height: 180px;
  left:-150px;
  border-width: 200px 0 0 300px;
  border-color: transparent transparent transparent #3596da;
}

#envelope:hover #card {
  top:-20px;
}

#card{
  width:260px;
  height: 220px;
  position: absolute;
  top:70px;
  left:-130px;
  z-index: -1;
  background: #dcdcdc;
  border-radius: 5px;
  transition: top 0.5s ease-in-out;
  font: bold 1em/0.9em 'Open Sans Condensed', sans-serif;
  text-align: center;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  padding: 125px 0 60px 0;
  color: black;
  line-height: 1em;
}

#card p {
  width: 150px;
  margin: 0 auto;

}

#button{
  top: 25px;
  left: 90px;
  right: -25px;
  height: 50px;
  width: 100px;
 
  overflow: hidden;
  position: absolute;
}
</style>
</head>
<body>
<!-- partial:index.partial.html -->
<div id='envelope'>
  <div id='card'>
    <p>
      We're just friend<br> what are you saying??
    </p>
    <div id='button'>CLICK ME&hearts;</div>
  </div>
</div>
<!-- partial -->
  <script  src="./script.js"></script>

</body>
</html>
