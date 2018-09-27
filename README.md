# js
杨辉三角
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
    <title>text</title>
    <script type="text/javascript">
        document.write("<div style='text-align: center;'>");
        var a1=[1,1];
        var a2=[];
        for (var i=1;i<9;i++){
            for(var j=0;j<i;j++){
                if((j==0)||(j==i-1)){
                    a2[j]=1;
                }else {
                    a2[j]=a1[j-1]+a1[j];
                }
            }
            for (var s=0;s<i;s++){
                a1[s]=a2[s];
            }
            document.write(a2);
            document.write("<br />")
        }
    </script>
</head>
<body>

</body>
</html>
