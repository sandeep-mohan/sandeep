# sandeep
Develop a scheduler which submits the processes to the processor in the defined
scenario, and compute the scheduler performance by providing the
waiting time for process, turnaround time for process and average
waiting time and turnaround time.
CODE:
#include<stdio.h>
#include<conio.h>
temp=bt[i];
bt[i]=bt[j];
bt[j]=temp;
temp=p[i];
p[i]=p[j];
p[j]=temp;
}
}
}
wt[0]=0;
for(i=1;i<n;i++)
{
wt[i]=wt[i-1]+bt[i-1];
}
for(i=0;i<n;i++)
{
sum+=wt[i];
}
avg=(float)sum/n;
printf("\n Waiting time for each process is:-");
for(i=0;i<n;i++)
{
printf("\n Waiting time for process P%d is %d
sec.",p[i],wt[i]);
}
printf("\n Average waiting time will be %f sec.",avg);
getch();
return 0;
}
