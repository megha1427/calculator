# calculator
<html>
  <head>
    <title> calculator program </title>
  </head>
  <?php 
  $a1 = .POST['$a1'];
  $a2 = .POST['$a2'];
  $operator = .POST['$operator'];
  $result = ' ';
    if(is_numeric($a1) && is_numeric($a2))
      {
        switch($operator)
        {
          case 'add': 
            $result=$a1+$a2;
            break;
          case 'sub':
            $result=$a1-$a2;
            break;
          case 'mul':
            $result=$a1+$a2;
            break;
          case 'div':
            $result=$a1+$a2;
          }
      }
  ?>
 <body>
	  <form action="" method="post" />
             First Number<input type="number" name="first_num"  value="<?php echo $a1; ?>" /> 
             Second Number<input type="number" name="second_num" value="<?php echo $a2; ?>" /> 
             result<input type="number" name="result" value="<?php echo $result; ?>"> <b>Result</b
            ADD<input type="submit" name="operator" value="Add" />
            SUB<input type="submit" name="operator" value="Subtract" />
            MUL<input type="submit" name="operator" value="Multiply" />
            DIV<input type="submit" name="operator" value="Divide" />
 </body>
</html>
