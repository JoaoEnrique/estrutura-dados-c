Alocação de memória com C.

Código:
```c
#include <stdio.h>

int main(){
    int a = 10;
    int b, c;

    printf("&a = %p, a = %d\n", &a, a);
    printf("&b = %p, b = %d\n", &b, b);
    printf("&c = %p, c = %d\n\n", &c, c);

    b = 20;
    c = a + b;
    
    printf("&a = %p, a = %d\n", &a, a);
    printf("&b = %p, b = %d\n", &b, b);
    printf("&c = %p, c = %d\n", &c, c);
    return 0;
}
```

Saída:

```cmd
&a = 0061FF1C, a = 10
&b = 0061FF18, b = 0
&c = 0061FF14, c = 12529616

&a = 0061FF1C, a = 10
&b = 0061FF18, b = 20
&c = 0061FF14, c = 30
```