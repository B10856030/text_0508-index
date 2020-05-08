# B10856030.github.io/text_0508-index.html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>草飼牛點餐價格表</title>
    <style>
        h1,
        h2 {
            font-weight: bolder;
            text-align: center;
        }
        
        h1 {
            font-size: 36px;
            color: blue;
        }
        
        h2 {
            font-size: 28px;
            color: red;
        }
        
        table {
            margin: auto;
        }
        
        #tableCaption {
            border-style: dashed;
            border-width: 1px;
        }
        
        .content {
            color: green;
            font-family: Arial;
            font-size: 18px;
        }
        
        #tableTitle {
            font-weight: bolder;
            font-size: 18px;
            color: purple;
            text-align: center
        }
        
        td {
            border-style: dotted;
            border-width: 1px;
            padding: 10px;
            border-color: red;
            color: green;
        }
        
        .p {
            border-style: none;
            border-width: 1px;
            padding: 10px;
        }
    </style>
    <script>
        document.write("<h1>草飼牛點餐價格表");
        document.write("<br><h2>折扣內容:套餐 1/套餐 2/套餐 3 買一送一 (限數量為雙數，單數數不折扣)");
        document.write('<table id="tableCaption"');
        for (a = 1; a <= 5; a++) {
            document.write('<th><td class="p"></th>');

            for (a = 1; a <= 5; a++) {

                document.write('<td id="tableTitle">套餐' + a + '<br>' + 50 * a + '元');


            }
        }



        for (i = 1; i <= 7; i++) {
            document.write("<tr>");
            document.write('<td id="tableTitle">' + i);
            for (j = 1; j <= 5; j++) {
                if (i % 2 == 0 && j < 4) {
                    document.write('<td>原價:' + 50 * i * j + '<br>折扣後:' + 50 * i * j / 2 + '</td>');
                } else {
                    document.write('<td>' + 50 * i * j + '</td>');
                }
            }
            document.write("</tr>");
        }
    </script>
</head>

<body>

</body>

</html>
