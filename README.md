# abaju3
agmar 

 //Save Computer
        mysql_query("INSERT INTO `pokemon_speler` (`wild_id`, `user_id`, `opzak`, `opzak_nummer`, `karakter`, "
                                        . "`level`, `levenmax`, `leven`, `totalexp`, `expnodig`, `attack`, `defence`, `speed`, "
                                        . "`spc.attack`, `spc.defence`, `attack_iv`, `defence_iv`, `speed_iv`, `spc.attack_iv`, "
                                        . "`spc.defence_iv`, `hp_iv`, `attack_ev`, `defence_ev`, `speed_ev`, `spc.attack_ev`, "
                                        . "`spc.defence_ev`, `hp_ev`, `aanval_1`, `aanval_2`, `aanval_3`, `aanval_4`, `effect`, "
                                        . "`ei`, `ei_tijd`, `gevongenmet`) VALUES ('" . $new_computer['id'] . "', '" . $_SESSION['id'] . "', 'nee', '', "
                                        . "'" . $karakter['karakter_naam'] . "', '" . $premiacao['lv_pokemon'] . "', '"
                                        . $new_computer['hpstat'] . "', '" . $new_computer['hpstat'] . "', '" . $experience['punten']
                                        . "', '" . $experience['punten'] . "', '" . $new_computer['attackstat'] . "', '"
                                        . $new_computer['defencestat'] . "', '" . $new_computer['speedstat'] . "', '"
                                        . $new_computer['spcattackstat'] . "', '" . $new_computer['spcdefencestat'] . "', "
                                        . "'" . $attack_iv . "', '" . $defence_iv . "', '" . $speed_iv . "', '" . $spcattack_iv . "', "
                                        . "'" . $spcdefence_iv . "', '" . $hp_iv . "', '" . $new_computer_sql['effort_attack'] . "', "
                                        . "'" . $new_computer_sql['effort_defence'] . "', '" . $new_computer_sql['effort_spc.attack']
                                        . "', '" . $new_computer_sql['effort_spc.defence'] . "', '" . $new_computer_sql['effort_speed']
                                        . "', '" . $new_computer_sql['effort_hp'] . "', '" . $new_computer['aanval1'] . "', '"
                                        . $new_computer['aanval2'] . "', '" . $new_computer['aanval3'] . "', '" . $new_computer['aanval4']
                                        . "', '" . $new_computer_sql['effect'] . "', '1', '" . $tijd . "', 'Luxury ball')");

		   mysql_query("UPDATE `gebruikers` SET `Secret_key`=`Secret_key`-'1000' WHERE `user_id`='".$_SESSION['id']."'");
