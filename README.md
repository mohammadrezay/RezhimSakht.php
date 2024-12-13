# RezhimSakht.php
https://quera.org/problemset/20256?tab=description
<?php
$a = (string)readline("Enter 5 characters: ");
$red_counter = 0;
$yellow_counter = 0;
$green_counter = 0;
$aa = [];
$aa = preg_split('//u', $a, null, PREG_SPLIT_NO_EMPTY);
foreach($aa as $color){
	if($color == "R"){
		$red_counter += 1;
	}elseif($color == "Y"){
		$yellow_counter += 1;
	}elseif($color == "G"){
		$green_counter += 1 ;
	}
}
if($red_counter >= 3){
	echo "nakhor lite";
}elseif($red_counter >= 2 and $yellow_counter >= 2){
	echo "nakhor lite";
}elseif($green_counter == 0){
	echo "nakhor lite";
}else{
	echo "rahat baash";
}
