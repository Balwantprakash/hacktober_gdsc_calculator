# hacktober_gdsc_calculator
#include <stdio.h>

int main() {

  char bp;
  double first, second;
  printf("Enter an operator (+, -, *, /): ");
  scanf("%c", &bp);
  printf("Enter two operands: ");
  scanf("%lf %lf", &first, &second);

  switch (bp) {
    case '+':
      printf("%.1lf + %.1lf = %.1lf", first, second, first + second);
      break;
    case '-':
      printf("%.1lf - %.1lf = %.1lf", first, second, first - second);
      break;
    case '*':
      printf("%.1lf * %.1lf = %.1lf", first, second, first * second);
      break;
    case '/':
      printf("%.1lf / %.1lf = %.1lf", first, second, first / second);
      break;
    default:
      printf("Error! operator is not correct");
  }
