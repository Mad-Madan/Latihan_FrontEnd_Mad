# Latihan_FrontEnd_Mad
This is my first repository in github
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Latihan 1</title>
    <link rel="stylesheet" href="DataTables/datatables.min.css">
</head>
<body>
   <table id="contoh" class="table">
        <thead>
             <tr>
                 <th width="5%">No</th>
                 <th width="40%">Nama</th>
                 <th width="25%">Kelas</th>
                 <th width="20%">Alamat</th>
                 <th width="15%">No HP</th>
             </tr>
        </thead>
   </table>
   <script src="DataTables/jQuery-3.6.0/jquery-3.6.0.min.js"></script>
   <script src="DataTables/datatables.min.js"></script>
   <script>
         $(function(){
            // var data = [
            //                 ["1", "Ismet", "XII RPL 2", "CPH", "083176180869"],
            //                 ["2", "Ismet", "XII RPL 2", "CPH", "083176180869"],
            //            ];

            var data = [];

            for (let i = 0; i < 5; i++) {
                data.push([i]);
              for(let j = 0; j < 5; j++){
                data[i].push(j);
              }
            }

           $("#contoh").DataTable({
              responsive : true,
              data : data
           });
         });
   </script>

</body>
</html>
