# Punkte-Klaptafel-Badminton
Punkte zählen

<!doctype html>
<html>
<head>
    <title>Vu's klapttabffel</title>
        <meta charset="utf-8" />
        <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
    <style type="text/css">
        
        .fetteText {
            font-weight:bold;
        }
        #bigbox{
            
        }
        
        #box1{
            width: 400px;
            height: 400px;
            float: left;
            background-color: burlywood;
        }

        #box1left{
            margin: 50px ;
            height: 200px;
            border: 10px  solid black;
            padding: 5px;
            flex: 1;
            background-color: white;
        }

        #minus1{
            width: 200px;
            height: 50px;
        }
        #plus1{
            width: 200px;
            height: 50px;
            float: left;
        }

        #box2{
            width: 400px;
            height: 400px;
            float: left;
            background-color: rgb(135, 219, 222);
        }
        #box2right{
            margin: 50px ;
            height: 200px;
            border: 10px  solid black;
            padding: 5px;
            flex: 1;
            background-color: white;
        }
        #minus2{
            width: 200px;
            height: 50px;
        }
        #plus2{
            width: 200px;
            height: 50px;
            float: left;
        }
        #nummerLeft{
            color:black;
            text-decoration:none;
            font-size:150px;
            margin: 12px 50px 0px 100px;
            
        }

        #nummerRight{
            color:black;
            text-decoration:none;
            font-size: 150px;
            margin: 12px 50px 0px 100px;
        }
        .buttonSize{
            background-color: goldenrod;
            color: black;
            font-size: 40px;
            line-height: 40px;
            font-weight: bold;
            
            
        }
    </style>

</head>
<body>

    <div id="bigbox">
        <div id="box1">
            <div id="box1left">

                <p class="fetteText" id="nummerLeft">0</p>

            </div>
            <button class="buttonSize"id="minus1">-</button>
            <button class="buttonSize"id="plus1">+</button>
        </div>


        <div id="box2">
            <div id="box2right">

                <p class="fetteText" id="nummerRight">0</p>

            </div>
            <button class="buttonSize" id="minus2">-</button>
            <button class="buttonSize" id="plus2">+</button>

        </div>
    </div>
    
    
    <script type="text/javascript">
       
        var punktLeft=0;
        var punktRight=0;

        document.getElementById("plus1").onclick=function(){
            if(punktLeft<30){
            punktLeft=punktLeft + 1;
            document.getElementById("nummerLeft").innerHTML=punktLeft;
            } else {
                alert("Spiel ist vorbei");
                
            }
        }

        document.getElementById("minus1").onclick=function(){
            if(punktLeft>0){
                punktLeft=punktLeft-1;
                document.getElementById("nummerLeft").innerHTML=punktLeft;
            }else{}
        }

        document.getElementById("plus2").onclick=function(){
            if(punktRight<30){
            punktRight=punktRight + 1;
            document.getElementById("nummerRight").innerHTML=punktRight;
            } else {
                alert("Spiel ist vorbei");
            }
        }

        document.getElementById("minus2").onclick=function(){
            if(punktRight>0){
                punktRight=punktRight-1;
                document.getElementById("nummerRight").innerHTML=punktRight;
            }else{}
        }
        

    </script>



</body>


</html>
