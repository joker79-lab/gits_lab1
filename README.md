# gits_lab1
<?php
echo "Mini Calculator\n";
echo "1. Addition\n";
echo "2. Subtraction\n";
echo "3. Multiplication\n";
echo "4. Division\n";

$choice = readline("Enter your choice (1-4): ");
$num1 = readline("Enter first number: ");
$num2 = readline("Enter second number: ");

switch ($choice) {
    case 1:
        echo "Result: " . ($num1 + $num2);
        break;

    case 2:
        echo "Result: " . ($num1 - $num2);
        break;

    case 3:
        echo "Result: " . ($num1 * $num2);
        break;

    case 4:
        if ($num2 != 0) {
            echo "Result: " . ($num1 / $num2);
        } else {
            echo "Error: Cannot divide by zero.";
        }
        break;

    default:
        echo "Invalid choice.";
}
?>