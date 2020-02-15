# zhenia.github.io
#include <stdio.h>



  typedef struct{ 
       int day;
       int month;
       int year;
    }date;
typedef struct{
    char *name;
    date arrival;
    int room;
    date departure
}Vasa;



int main(void)
{
  
    
  Vasa **a = NULL;
  int n = 0;
  
  n=2;
  a=(Vasa **)realloc(a, sizeof(Vasa *) * n);
  a[0] = NULL;
  a[0] = (Vasa *)realloc(a[0], sizeof(Vasa));
  a[0]->name = NULL;
  a[0]-> name = (char *)realloc(a[0]-> name, sizeof(char) *41);
  printf ("Введите ФИО ");
  scanf("%[^\t\n]s", a[0]->name);
  printf ("Введите дату заезда:\nДень ");
  scanf("%d", &a[0]->arrival.day);
  printf ("Месяц ");
  scanf("%d", &a[0]->arrival.month);
  printf ("Введите номер комнаты ");
  scanf("%d", &a[0]->room);
  *a[1]=*a[0];
  printf("ФИО: %s, Дата прибытия:%02d.%02d.%04d, Номер комнаты: %d\n");
  a[1]->name,a[1]->arrival.day,a[1]->arrival.month,a[1]->arrival.year,a[1]->room);
  
  a[0]->name = (char *)realloc(a[0]->name,0);
  a[0] = (Vasa *)realloc(a[0],0);
  a[1] = (Vasa *)realloc(a[1],0);
  date arrival= {20, 03, 2020};
  printf("day:%s \t month:%s \t year: %d", arrival.day, arrival.month, arrival.age);

    return 0;
}
