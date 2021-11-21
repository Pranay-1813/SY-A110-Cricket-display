#include<stdio.h>
struct cricket
{
  int runs_scored,wickets;
  float avg;
  char name[20];
}player[25];
int main(void)
{
  int n,ch;
  printf("Enter the total no of players:\n");
  scanf("%d",&n);
  
  for(int i=1;i<=n;i++)
  {
    printf("Enter the player %d \n\nTheir information(name runs_scored wickets avg):\n",i);
    scanf("%s %d %d %f", player[i].name,&player[i].runs_scored,&player[i].wickets,&player[i].avg);
  }
  printf("Enter the choice:\n0,sort\n1,search\n2,show");
  scanf("%d",&ch);
  switch(ch)
  {
    case 0:{}
    break;
    case 1:{}
    break;
    case 2:
    {
      printf("player_Name Runs_scored Wickets Avg\n");
      for(int i=1;i<=n;i++)
      {
        printf("%s\t\t\t %d\t%d\t\t%.2f\n", player[i].name,player[i].runs_scored,player[i].wickets,player[i].avg);
      }
    }

  }
}
