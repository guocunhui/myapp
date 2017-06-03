<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <style>
        *{
            margin: 0;
            padding: 0;;
        }
        .box{
            display: flex ;
            width: 99%;
            height: 600px;
            border:1px solid black;
            margin: 0 auto;
        }
        .box1{
            width: 50%;
            height: 600px;
            border:1px solid red;
        }
        .input{
            width: 100%;
            height: 598px;
            border:1px solid red;
            background-color: #2d3237 ;
        }
    </style>
    <script src="jquery-1.11.3.min.js"></script>
    <script>
        $(function(){
            $("input").click(function(){
                var content=$("input:text").val();
                $("ul").prepend("<li>"+content+"</li>")
            })
        })
    </script>
</head>
<body>
<div class="box">
    <div class="box1" type="text">
        <input type="text" value="" class="input">
    </div>
    <div class="box1"></div>
</div>
</body>
</html>
