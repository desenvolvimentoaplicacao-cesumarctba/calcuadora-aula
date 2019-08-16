//# calcuadora-aula
<?php;
include 'polyfill.php';

echo '**** Calculadora ****' . PHP_EOL;
echo '**** 1 - Adicao ****' . PHP_EOL;
echo '**** 2 - Divisao ****' . PHP_EOL;
echo '**** 3 - Multiplicacao ****' . PHP_EOL;
echo '**** 4 - Subtracao ****' . PHP_EOL;

$operacao = readline("Escolha a Operacao:" . PHP_EOL);	
$valor1 = readline("Digite o primeiro valor:" . PHP_EOL);	
$valor2 = readline("Digite o segundo valor:" . PHP_EOL);

$resultado = 0;

switch ($operacao) {
	case 1:
		$resultado = $valor1 + $valor2;
		break;
	case 2:
		$resultado = $valor1 / $valor2;
		break;
	case 3:
		$resultado = $valor1 * $valor2;
		break;
	case 4:
		$resultado = $valor1 - $valor2;
		break;	
	default:
		echo "Operacao Invalida!" . PHP_EOL;
		return 0;
}	

echo "Resultado:  " . $resultado . PHP_EOL;
