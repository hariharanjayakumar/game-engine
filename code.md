//Project originally designed in Turbo C++
#include<string.h>
#include<math.h>
#include<iostream>
#include<conio.h>
#include<stdio.h>
#include<stdlib.h>
#include<time.h>
#include<dos.h>
#include<graphics.h>
using namespace std;
void quit()
{ int gdriver = DETECT, gmode, errorcode;

initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
delay(1000);
cleardevice();
 settextstyle(3,0,1);
setbkcolor(6);
cleardevice();
setcolor(2);
for(int i=1;i<=150;i++)
{moveto(250,i);
outtext("A PROJECT BY");
delay(10);
if(i<150)
{cleardevice();}
}
moveto(50,180);
outtext("G.ASHWIN KRISHNAN");
delay(500);
moveto(280,180);
outtext("HARIHARAN.J");
delay(500);
moveto(430,180);
outtext("ADITHYA NARASIMHAN");
delay(1000);
for(i=580;i>=200;i--)
{
moveto(220,i);
outtext("THANK YOU FOR VIEWING.. ");
delay(10);
if(i>200)
cleardevice();}
delay(1000);
exit(0);
}
void tictac();
void bounce();
void foot();
void flappy();
void intromain()
{int gdriver = DETECT, gmode, errorcode;
initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
cleardevice();
for(int i=0;i<=360;i++)
{pieslice(300,250,0,i,150);
delay(5);
}
for(int y=280;y>180;y--)
	 for(int x=80;x<=310;x++)

		if(y>265&&x<130||y<195&&x<130||x<90||x>120&&x<130&&y>230||x>100&&x<=120&&y>230&&y<245||
		 x>140&&x<150||x>180&&x<190||y<195&&x>140&&x<190||y<235&&y>220&&x<190&&x>140||
		 x>200&&x<213||x>237&&x<250||y<195&&x>200&&x<250||x>218&&x<232&&y>=195&&y<240||
		 x>260&&x<272||y<195&&x>260||y>265&&x>260||y>225&&y<240&&x>=270&&x<300)

		       {putpixel(x,y,4);
			delay(0);}


for(y=180;y<280;y++)
	for(x=350;x<615;x++)
		if(x<363||x<390&&y<195||x<390&&y<280&&y>265||
		   x<415&&x>400||
		   x>425&&x<440||x<465&&x>425&&y<195||x<465&&x>425&&y<220&&y>205||x>425&&x<465&&y<240&&y>225||x>450&x<465&&y>225||x>450&&x<465&&y<220||
		   x>475&&x<490||x>475&&x<515&&y<195||x>475&&x<515&&y>265||
		   x>525&&x<540||x>525&&x<565&&y>265||
		   x>575&&x<590||x>575&&y<195||x>575&&x<600&&y<237&&y>222||x>575&&y>265)
		   {putpixel(x,y,1);
		   delay(0);
		   }
getch();

cleardevice();
int a=1;
setcolor(5);
rectangle(10,125,190,450);
while(1)
{setbkcolor(0);
for( y=280-160;y>180-160;y--)
	 for( x=80;x<=310;x++)

		if(y>265-160&&x<130||y<195-160&&x<130||x<90||x>120&&x<130&&y>230-160||x>100&&x<=120&&y>230-160&&y<245-160||
		 x>140&&x<150||x>180&&x<190||y<195-160&&x>140&&x<190||y<235-160&&y>220-160&&x<190&&x>140||
		 x>200&&x<213||x>237&&x<250||y<195-160&&x>200&&x<250||x>218&&x<232&&y>=195-160&&y<240-160||
		 x>260&&x<272||y<195-160&&x>260||y>265-160&&x>260||y>225-160&&y<240-160&&x>=270&&x<300)

		       {putpixel(x,y,4);
			delay(0);}


for(y=180-160;y<280-160;y++)
	for(x=350;x<615;x++)
		if(x<363||x<390&&y<195-160||x<390&&y<280-160&&y>265-160||
		   x<415&&x>400||
		   x>425&&x<440||x<465&&x>425&&y<195-160||x<465&&x>425&&y<220-160&&y>205-160||x>425&&x<465&&y<240-160&&y>225-160||x>450&x<465&&y>225-160||x>450&&x<465&&y<220-160||
		   x>475&&x<490||x>475&&x<515&&y<195-160||x>475&&x<515&&y>265-160||
		   x>525&&x<540||x>525&&x<565&&y>265-160||
		   x>575&&x<590||x>575&&y<195-160||x>575&&x<600&&y<237-160&&y>222-160||x>575&&y>265-160)
		   {putpixel(x,y,1);
		   delay(0);
		   }
  if(a>=1&&a<=3)
  {
int p[134]={270,105,265,106,262,111,260,118,263,124,263,128,260,128,260,132,250,138,223,165,208,176,204,178,201,181,
	    204,189,206,186,206,190,213,184,218,180,253,155,258,163,240,197,233,203,225,215,200,238,198,243,200,248,
	    205,248,230,225,245,217,265,203,278,204,280,210,280,218,270,233,268,247,258,263,255,270,275,277,287,277,291,274,283,270,275,260,
	    300,210,300,200,292,172,291,140,305,127,304,125,327,103,337,99,339,96,335,98,338,92,335,94,338,89,332,92,334,88,333,87,325,92,322,98,302,115,278,128,277,125,280,119,280,110,276,106,270,105};
for(int i=1;i<134;i+=2)
    {p[i]+=50;
     p[i-1]+=60;}
setfillstyle(0,3);
setcolor(4);
fillpoly(67,p);
rectangle(480,300,580,310);
circle(530,250,5);
line(75,200,75,350);
line(125,200,125,350);
line(25,250,175,250);
line(25,300,175,300);
settextstyle(1,0,3);
outtextxy(140,310,"O");
outtextxy(90,260,"X");
outtextxy(40,210,"O");
setcolor(4);
setfillstyle(1,4);
settextstyle(3,0,4);
outtextxy(480,400,"BOUNCE");
outtextxy(215,400,"STREET SOCCER");
outtextxy(20,400,"TICTACTOE");
}
else
{setfillstyle(1,14);
fillellipse(100-3,250,22,20);
setfillstyle(1,4);
fillellipse(100+16,250+2,13,4);
fillellipse(100+16,250+8,13,4);
setfillstyle(1,15);
fillellipse(100+15,250-8,6,7);
circle(116,242,5);
setcolor(4);
outtextxy(50,400,"FLAPPY");
}
if(kbhit())
{cleardevice();
char v=getch();
if(v=='a'&&a>1)
a--;
else if(v=='d'&&a<4)
a++;
else if(v=='q')
break;
else if(v==13)
{if(a==1)
tictac();
else if(a==2)
foot();
else if(a==3)
bounce();
else
flappy();
}
setcolor(5);
if(a==1)
rectangle(10,125,190,450);
if(a==2)
rectangle(200,125,450,450);
if(a==3)
rectangle(460,125,620,450);
if(a==4)
rectangle(10,125,190,450);
}
}
}
void BIRD(int x,int y,int z)
{setcolor(0);
setfillstyle(1,14);
fillellipse(x-3,y,22,20);
setfillstyle(1,4);
fillellipse(x+16,y+2,13,4);
fillellipse(x+16,y+8,13,4);
setfillstyle(1,15);
fillellipse(x+15,y-8,6,7);
setfillstyle(1,4);
if(z<6)
fillellipse(x-25,y+5,15,6);
else
fillellipse(x-25,y-5,15,6);
setfillstyle(1,1);
fillellipse(x+19,y-9,2,2);
setcolor(15);

}
void flappy()
{ int x1,y1,y2,x2,x=190,y=200,jump=0,scr=0;
int gdriver = DETECT, gmode, errorcode,sa=0,sv=0;
char r[5];

initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
while(1)
{cleardevice();
setbkcolor(14);
settextstyle(4,0,5);
setcolor(4);
outtextxy(200,50,"FLAPPY BIRD");
settextstyle(4,0,4);
outtextxy(150,100,"(1)PLAY");
outtextxy(150,150,"(2)INSTRUCTIONS");
outtextxy(150,200,"(3)HIGHSCORE");

int ch=getch();
if(ch=='1')
{scr=0;
settextstyle(6,0,3);
cleardevice();
randomize();
outtextxy(100,200,"PRESS 'SPACE' KEY TO MAKE IT JUMP");
delay(1000);
x1=324;x2=-50;
y1=random(200)+100;
getch();
int z=0;
while(1)
{
z++;
 if(x1+50<=0)
  {
   y1=100+random(200);x1=650; }
   if(x2+50<=0)
   {
   y2=100+random(200);x2=650;}
   x1-=2;x2-=2;
setactivepage(sa);
setbkcolor(9);
BIRD(x,y,z);
setfillstyle(1,2);
bar(x1,0,x1+50,y1);
bar(x1,y1+100,x1+50,400);
bar(x2,0,x2+50,y2);
bar(x2,y2+100,x2+50,400);
line(0,400,650,400);
itoa(scr,r,10);
outtextxy(350,420,r);
setvisualpage(sv);
if(sa==0)
sa=1;
if(sv==0)
sv=1;
if(sv==1)
sv=0;
if(sa==1)
sa=0;
delay(25);
cleardevice();

if(kbhit())
{char ch=getch();
if(ch=='q')
break;
else if(ch==32)
jump-=10;
}
if(y>=380||y<=20)
break;
if(x+18>=x1&&x-18<=x1+50&&(y+18>=y1+100||y-18<=y1))
break;
if(x+18>=x2&&x-18<=x2+50&&(y+18>=y2+100||y-18<=y2))
break;
if(jump<0)
{jump++;
y+=jump;}
else
y+=4;
setfillstyle(1,6);
bar(0,400,650,500);
if(x-20==x1+50||x-20==x2+50)
scr++;

if(z==10)
z=0;
}
settextstyle(3,0,4);
outtextxy(200,200,"YOU HAVE CRASHED!!!");
outtextxy(220,250,"SCORE:");
outtextxy(330,250,r);
getch();
getch();
cleardevice();
}
else if(ch=='2')
{cleardevice();
settextstyle(1,0,6);
setcolor(4);
outtextxy(150,5,"INSTRUCTIONS");
settextstyle(4,0,4);
outtextxy(20,100,"Press 'space' key to make your bird fly");
outtextxy(5,150," higher. the bird dies if it either crashes");
outtextxy(5,200," on on the hurdles or the cieling or the floor");
outtextxy(5,250," good luck for your gaming!!!");
getch();

}
else if(ch=='3');
else break;
}
cleardevice();
}


void select(int x,int y)
{setcolor(5);
if(x==1&&y==1)
rectangle(105,105,195,195);
else if(x==2&&y==1)
rectangle(205,105,295,195);
else if(x==3&&y==1)
rectangle(305,105,395,195);
else if(x==1&&y==2)
rectangle(105,205,195,295);
else if(x==2&&y==2)
rectangle(205,205,295,295);
else if(x==3&&y==2)
rectangle(305,205,395,295);
else if(x==1&&y==3)
rectangle(105,305,195,395);
else if(x==2&&y==3)
rectangle(205,305,295,395);
else if(x==3&&y==3)
rectangle(305,305,395,395);
}
void board(int a[][3])
{setcolor(3);
rectangle(100,100,400,400);
line(200,100,200,400);
line(300,100,300,400);
line(100,200,400,200);
line(100,300,400,300);
settextstyle(3,0,6);
setcolor(4);
for(int i=0;i<3;i++)
for(int j=0;j<3;j++)
{if(a[i][j]!=0)
 {moveto(i*100+140,j*100+120);
  if(a[i][j]==1)
  outtext("X");
  else
  outtext("O");
 }
}
}
int check(int a[][3])
{if(a[0][0]==1&&a[0][1]==1&&a[0][2]==1)
 return 1;
 else if(a[1][0]==1&&a[1][1]==1&&a[1][2]==1)
 return 1;
 else if(a[2][0]==1&&a[2][1]==1&&a[2][2]==1)
 return 1;


 else if(a[0][0]==1&&a[1][0]==1&&a[2][0]==1)
 return 1;
 else if(a[0][1]==1&&a[1][1]==1&&a[2][1]==1)
 return 1;
 else if(a[0][2]==1&&a[1][2]==1&&a[2][2]==1)
 return 1;


 else if(a[0][0]==1&&a[1][1]==1&&a[2][2]==1)
 return 1;
 else if(a[2][0]==1&&a[1][1]==1&&a[0][2]==1)
 return 1;



 else if(a[0][0]==2&&a[0][1]==2&&a[0][2]==2)
 return 2;
 else if(a[1][0]==2&&a[1][1]==2&&a[1][2]==2)
 return 2;
 else if(a[2][0]==2&&a[2][1]==2&&a[2][2]==2)
 return 2;


 else if(a[0][0]==2&&a[1][0]==2&&a[2][0]==2)
 return 2;
 else if(a[0][1]==2&&a[1][1]==2&&a[2][1]==2)
 return 2;
 else if(a[0][2]==2&&a[1][2]==2&&a[2][2]==2)
 return 2;


 else if(a[0][0]==2&&a[1][1]==2&&a[2][2]==2)
 return 2;
 else if(a[2][0]==2&&a[1][1]==2&&a[0][2]==2)
 return 2;

 else
 return 0;
}
int draw(int a[][3])
{int f=0;
 for(int i=0;i<3;i++)
 for(int j=0;j<3;j++)
 if(a[i][j])
 f++;
 if(f==9)
 return 1;
 else
 return 0;
}
void tictac()
{int gdriver = DETECT, gmode, errorcode;
int midx, midy, i;
initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
cleardevice();
setcolor(2);
for(i=0;i<450;i+=2)
{if(i<449);
cleardevice();
line(i-300,175,i,175);
 line(i-300,275,i,275);
 line(350,i-100,350,i-350);
 line(250,i-100,250,i-350);
 delay(10);
  }
  setcolor(5);
  settextstyle(4,0,5);
  delay(500);
  outtextxy(290,200,"X");
  delay(500);
  outtextxy(400,100,"O");
  delay(500);
  outtextxy(180,100,"X");
  delay(500);
  outtextxy(180,300,"O");
  delay(500);
  outtextxy(400,300,"X");
  delay(400);
  line(160,100,425,340);

  setcolor(4);
  settextstyle(7,0,5);
  delay(500);
  outtextxy(200,400,"T");
  delay(500);
  outtextxy(230,400,"I");
  delay(500);
  outtextxy(260,400,"C");
  delay(500);
  outtextxy(290,400,"T");
  delay(500);
  outtextxy(320,400,"A");
  delay(500);
  outtextxy(350,400,"C");
  delay(500);
  outtextxy(380,400,"T");
  delay(500);
  outtextxy(410,400,"O");
  delay(500);
  outtextxy(440,400,"E");





delay(2000);




do{cleardevice();
 setbkcolor(14);
  setcolor(4);
  settextstyle(3,0,5);
  outtextxy(200,50,"TICTACTOE");
  setcolor(2);
  rectangle(200,170,460,220);
  settextstyle(1,0,4);
  setcolor(2);
  outtextxy(200,175," 1.PLAY GAME");
  rectangle(200,225,460,275);
  outtextxy(210,230,"2.INSTRUCTIONS");
  rectangle(200,280,460,325);
  outtextxy(220,285,"3.EXIT");
  outtextxy(230,405,"enter choice:");
  char n=getch();
 if(n=='1')
 { setcolor(5);


 cleardevice();
  setbkcolor(0);
  setcolor(5);
  rectangle(205,205,295,295);

  int x=2,y=2,a[3][3]={0},z=0;
   while(1)
	  {board(a);
	   setcolor(4);
	   settextstyle(3,0,5);
	   outtextxy(410,200,"TURN:");
	   setcolor(6);
	   settextstyle(4,0,4);
	   if(z%2==0)
	   outtextxy(405,250,"PLAYER 1");
	   else
	   outtextxy(405,250,"PLAYER 2");
	   if(check(a)==1)
	   {moveto(150,410);
	    outtext("PLAYER 1 WINS!!!");
	    delay(3000);
	    break;}
	   if(check(a)==2)
	    {moveto(150,410);
	     outtext("PLAYER 2 WINS!!!");
	     delay(3000);

	     break;
	    }
	   if(draw(a))
	   {outtextxy(150,410,"GAME IS A DRAW!!!");
	    delay(3000);
	    break;
	   }
	  if(kbhit())
	  {cleardevice();
	  char c=getch();
	  if(c=='a'&&x>1)
	  x--;
	  else if(c=='d'&&x<3)
	  x++;
	  else if(c=='w'&&y>1)
	  y--;
	  else if(c=='s'&&y<3)
	  y++;
	  else if(c=='q')
	  {outtextxy(250,50,"PAUSED");
	  outtextxy(150,250,"RUNNING AWAY(y/n)");
	  char h=getch();
	  if(h=='y'||h=='Y')
	  break;
	  cleardevice();
	  }
	  if(c=='m'&&a[x-1][y-1]==0)
	  {z++;
	  if(z%2)
	  a[x-1][y-1]=1;
	  else
	  a[x-1][y-1]=2;
	  }

     select(x,y);

   }

 }
 }
 if(n=='3')
 break;
 if(n=='2')
 {cleardevice();
 setbkcolor(14);
 setcolor(4);
 settextstyle(5,0,5);
 outtextxy(170,25,"INSTRUCTIONS");
 settextstyle(1,0,3);
 setcolor(2);
 outtextxy(50,100,"the players have to try and put their mark");outtextxy(50,130,"(x or o)in 3 consecutive boxes either vertically");outtextxy(50,160,"or horizontally or diagonally while blocking the");outtextxy(50,190,"opponent from doing the same");
 outtextxy(50,220,"movements:");
 outtextxy(50,250,"A -> LEFT    D -> RIGHT     W -> UP");
 outtextxy(50,280,"S -> DOWN   M -> MARK    Q->STOP GAME");
 getch();

 }
 }while(1);
 cleardevice();
 }
 struct bounplay
{char name[20];
int score;
}player[20];
void bounce()
{int o=-1;
char z;
for(int i=0;i<20;i++)
strcpy(player[i].name,"no name");
 int d=DETECT,m;
   initgraph(&d,&m,"c:\\turboc3\\bgi");
   float x=1,y=0.00000,j=.5,count=.1;
   float r=15;
   setcolor(14);
   line(0,215,650,215);
    sleep(1);
    for(int k=0;k<=7;k++)
     {

      for(float i=90;i<270;i+=10)
       {
	y=cos(((i*22/7)/180))/j;

	if(y>0)
	y=-y;
	x+=5;

	setcolor(14);
	setfillstyle(1,14);
	circle(x,y*100+200,r);
	floodfill(x,y*100+200,14);

       delay(100);

	setcolor(0);
	setfillstyle(1,0);
	circle(x,y*100+200,r);
	floodfill(x,y*100+200,0);
	setcolor(4);
	settextstyle(1,0,4);
	outtextxy(250,300,"Bounce");
       }

      j+=count;
      count+=.1;

     }
   getch();
do{cleardevice();
  setbkcolor(3);
  setcolor(4);
  settextstyle(7,0,6);
  moveto(250,20);
outtext("MENU");
delay(1000);
settextstyle(6,0,4);
moveto(100,100);
outtext("(1)PLAY GAME");
moveto(100,140);
delay(1000);
outtext("(2)INSTRUCTIONS");
delay(1000);
moveto(100,180);
outtext("(3)HIGHSCORE");
moveto(100,220);
delay(1000);
outtext("choose an option");
char c=getch();
if(c=='1')
{
clrscr();
o++;
gotoxy(27,5);
cleardevice();
setcolor(4);
for( i=0;i<500;i++)
{outtextxy(60+i,50,"#");
outtextxy(60+i,400,"#");
}
for(i=0;i<350;i++)
{outtextxy(60,i+50,"#");
outtextxy(560,i+50,"#");
}
setcolor(3);
setfillstyle(9,3);
bar(280,385,350,395);
setcolor(1);
setfillstyle(1,1);
fillellipse(310,374,10,10);
x=280;
int dir=1;
int xb=310,yb=374,ball=1,scr=0;
getch();
while(1)
{
delay(5);
setcolor(0);
setfillstyle(1,0);
bar(65,55,555,395);
settextstyle(4,0,2);
setcolor(4);
outtextxy(590,100,"score");
char sc[5];
itoa(scr,sc,10);
outtextxy(600,130,sc);
setcolor(1);
setfillstyle(1,1);
fillellipse(xb,yb,10,10);
setcolor(3);
setfillstyle(9,3);
bar(x,385,x+70,395);
if(kbhit())
{char f=getch();
if(f=='a')
dir=1;
if(f=='d')
dir=2;
if(f=='q')
/*{cleardevice();
settextstyle(4,0,5);
outtextxy(200,50,"GAME PAUSED");
settextstyle(4,0,3);
outtextxy(200,250,"WANT TO STOP PLAYING?(y/n)");
char y=getch();
if(y=='y'||y=='Y')*/
break;
/*else
{cleardevice();
setcolor(4);
for(int u=0;u<500;u++)
{outtextxy(60+u,50,"#");
outtextxy(60+u,400,"#");
}
for(u=0;u<350;u++)
{outtextxy(60,u+50,"#");
outtextxy(560,u+50,"#");
}
}
} */
}
if(dir==1&&x>66)
x--;
else if(dir==2&&x<485)
x++;
if(xb==75&&ball==1)
ball=2;
if(xb==75&&ball==4)
ball=3;
if(xb==545&&ball==2)
ball=1;
if(xb==545&&ball==3)
ball=4;
if(yb==65&&ball==1)
ball=4;
if(yb==65&&ball==2)
ball=3;
if(yb==374&&ball==3&&xb>=x-5&&xb<x+75)
{ball=2;scr++;
setfillstyle(1,0);
bar(600,120,650,150);}
if(yb==374&&ball==4&&xb>=x-5&&xb<x+75)
{ball=1;scr++;
setfillstyle(1,0);
bar(600,120,650,150);
}
if(yb==380)
{settextstyle(4,0,5);
outtextxy(200,200,"GAME OVER");
player[o].score=scr;
getch();
break;
}
if(ball==1)
{xb--;yb--;}
if(ball==2)
{xb++;yb--;}
if(ball==3)
{xb++;yb++;}
if(ball==4)
{xb--;yb++;}

}}
if(c=='3')
{bounplay t;
closegraph();
for(i=0;i<19;i++)
for(int j=0;j<19-i;j++)
if(player[j].score<player[i+1].score)
{t=player[j];
player[j]=player[j+1];
player[j+1]=t;
}
for(i=0;i<15;i++)
cout<<player[i].name<<"\t\t"<<player[i].score<<'\n';
getch();
int gdriver = DETECT, gmode, errorcode;
initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
}
if(c=='q')
break;
}while(1);
cleardevice();
}





struct Team
{int x,y;
  char name[10];
  int goalcount;};

Team A[3]={420,435,"ARAVIND",0,520,335,"HARIHARAN",0,300,335,"JOE",0};//TEAM CONTROLLED BY THE USER
Team B[3]={420,30,"VENKATESH",0,520,90,"NARASIMAN",0,300,90,"DHANARAAJ",0};

int xb=420,yb=250;//COORDINATES OF BALL
int x=A[1].x,y=A[1].y,xs=A[2].x,ys=A[2].y;//x AND y ARE THE COORDINATES OF THE PRIMARY PLAYER.. THE PRIMARY PLAYER IS THE ONE WHO MOVES
//xs AND ys ARE THE CORDINATES OF THE SECOND PLAYER
//IMPORTANT:- x,xs,y AND ys ARE USED TO FACILITATE PASSING AND NAVIGATION AND ARE NOT THE ACTUAL PLAYER COORDINATES
int i,k1=1,k2=1;
char minute[5],second[5];
int goal1=0,goal2=0;

void restriction()
{
if(xb>631)  xb=631;
if(xb<200) xb=200;
if(yb>465) yb=465;
if(yb<10) yb=10;


//GOALKEEPER1 RESTRICTIONS
if(A[0].x<=340) {A[0].x=342;}
if(A[0].x>= 480){A[0].x=478;}
if(A[0].y<=400) {A[0].y=402;}
if(A[0].y>=465) {A[0].y=462;}

	    //GOALKEEPER2 RESTRICTIONS
	      if(B[0].x<=340) {B[0].x=342;}
	      if(B[0].x>= 480){B[0].x=478;}
	      if(B[0].y<=20) {B[0].y=22;}
	      if(B[0].y>=75) {B[0].y=73;}
}

inline void playerbody(int xi,int yi)
{
bar(xi-4,yi-13,xi+4,yi-5);//man's body
pieslice(xi,yi-15,0,360,2);//man's head
line(xi-4,yi-13,xi-9,yi-8);//left hand
line(xi+4,yi-13,xi+9,yi-8);//right hand
line(xi-4,yi-5,xi-6,yi);//left leg
line(xi+4,yi-5,xi+6,yi);//right leg
}

void swap()//FUNCTION TO SWAP PRIMARY AND SECONDARY PLAYER
{int t=x;
 x=xs;
 xs=t;
 t=y;
 y=ys;
 ys=t;
}

void navigation(int i,char action)//FUNCTION TO MOVE THE PRIMARY PLAYER AROUND
{
if(action=='a'||action=='A')
    {x-=2;
    A[i].x-=2;
    if(pow(x-xb,2)+pow(y-yb,2)<=40)
	   xb-=2;
    }
if(action=='d'||action=='D')
    {x+=2;
     A[i].x+=2;
    if(pow(x-xb,2)+pow(y-yb,2)<=40)
	   xb+=2;
    }
if(action=='w'||action=='W')
    {y-=2;
     A[i].y-=2;
    if(pow(x-xb,2)+pow(y-yb,2)<=40)
	   yb-=2;
    }
if(action=='s'||action=='S')
    {y+=2;
     A[i].y+=2;
    if(pow(x-xb,2)+pow(y-yb,2)<=40)
	   yb+=2;
    }
}//navigation

int timer(clock_t start)
{clock_t end;
 end=clock();
unsigned long int timeelapsed=end-start;
return timeelapsed;
}


void pass(int xs=::xs,int ys=::ys)//FUNCTION TO PASS THE BALL FROM THE PRIMARY TO SECONDARY PLAYER
{
for(int i=1;i<=100;i++)// GUARD CODE B|
   {setfillstyle(1,2);
    bar(xb-2,yb-2,xb+2,yb+2);
    setfillstyle(1,7);

//HERE COME THE INNUMERABLE PASSING CONDITIONS WHICH STRIVE TO BRING PERFECTION INTO THIS GAME
	 if(abs(ys-yb) > 3*abs(xs-xb) || xs==xb){yb+=4*(ys-yb)/abs(ys-yb);}
    else if(abs(ys-yb) > 2*abs(xs-xb))          {xb+=4*(xs-xb)/abs(xs-xb);  yb+=12*(ys-yb)/abs(ys-yb);}
    else if(abs(ys-yb) > abs(xs-xb))            {xb+=4*(xs-xb)/abs(xs-xb);  yb+=8*(ys-yb)/abs(ys-yb);}
    else if(abs(xs-xb) > 3*abs(ys-yb) || ys==yb){xb+=4*(xs-xb)/abs(xs-xb);}
    else if(abs(xs-xb) > 2*abs(ys-yb))          {yb+=4*(ys-yb)/abs(ys-yb);  xb+=12*(xs-xb)/abs(xs-xb);}
    else if(abs(xs-xb) > abs(ys-yb))            {yb+=4*(ys-yb)/abs(ys-yb);  xb+=8*(xs-xb)/abs(xs-xb);}
    else if(abs(xs-xb) == abs (ys-yb))          {yb+=4*(ys-yb)/abs(ys-yb);  xb+=4*(xs-xb)/abs(xs-xb);}

    restriction();
    if(xs==::xs && ys==::ys)
	    {if(pow(B[1].x-xb,2)+pow(B[1].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=B[1].x+10;
	      yb=B[1].y-2;
	      break;}
	     if(pow(B[2].x-xb,2)+pow(B[2].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=B[2].x+10;
	      yb=B[2].y-2;
	      break;}
	      }
    else    {if(pow(A[1].x-xb,2)+pow(A[1].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=A[1].x+10;
	      yb=A[1].y-2;
	      break;}
	     if(pow(A[2].x-xb,2)+pow(A[2].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=A[2].x+10;
	      yb=A[2].y-2;
	      break;}
	      }


    pieslice(xb,yb,0,360,2);
    if(pow(xs-xb,2)+pow(ys-yb,2)<=625)//CONDITION WHEN THE BALL HAS REACHED THE SECONDARY PLAYER
	 {setfillstyle(1,2);
	  bar(xb-2,yb-2,xb+2,yb+2);
	  if(xb<=xs)
	       xb=xs-10;
	  else xb=xs+10;
	  yb=ys;
	  swap();
	  break;
	  }
delay(20);
}//for loop
pieslice(xb,yb,0,360,2);
}

void longball()
{
randomize();
int destin1,xdirect;
//destin1 IS THE POTENTIAL DISPLACEMENT OF THE BALL AND xdirect DECIDES DIRECTION OF BALL
destin1=random(170)+100;
//xdirect=random(2);
for(int i=0;i<110;i++)
   {setfillstyle(1,2);
    bar(xb-2,yb-2,xb+2,yb+2);
    setfillstyle(1,7);
    if(destin1<635-x)
	 xb+=4;
    else if (destin1<200-xb)
	 xb-=4;
    yb-=6;
    pieslice(xb,yb,0,360,2);
    if(abs(yb-y)>destin1-10)//CONDITION WHEN THE BALL HAS REACHED THE DESTINATION
	 {setfillstyle(1,2);
	  bar(xb-2,yb-2,xb+2,yb+2);
	  break;
	  }
    restriction();
    if(yb==10 || xb==200 || xb==630)
	    break;
    delay(20);
    }
}

void goalkeeper(Team &A)
{
     if(xb>A.x) A.x+=4;
else if(xb<A.x) A.x-=4;
     if(yb-A.y<50 && yb>A.y) A.y+=4;
else if(A.y-yb<50 && A.y>yb) A.y-=4;

}

void shoot1(int a,Team &C)
{
randomize();
int ys1=7+a;
int xs1=360+random(100);
for(int i1=1;i1<=115;i1++)//GUARD CODE
   {setfillstyle(1,2);
    bar(xb-2,yb-2,xb+2,yb+2);
    setfillstyle(1,7);

//HERE COME THE INNUMERABLE PASSING CONDITIONS WHICH STRIVE TO BRING PERFECTION INTO THIS GAME
	 if(abs(ys1-yb) >  3*abs(xs1-xb) || xs1==xb){yb+=4*(ys1-yb)/abs(ys1-yb);}
    else if(abs(ys1-yb) >  2*abs(xs1-xb))          {xb+=4*(xs1-xb)/abs(xs1-xb);  yb+=12*(ys1-yb)/abs(ys1-yb);}
    else if(abs(ys1-yb) >  abs(xs1-xb))            {xb+=4*(xs1-xb)/abs(xs1-xb);  yb+=8*(ys1-yb)/abs(ys1-yb);}
    else if(abs(xs1-xb) >  3*abs(ys1-yb) || ys1==yb){xb+=4*(xs1-xb)/abs(xs1-xb);}
    else if(abs(xs1-xb) >  2*abs(ys1-yb))          {yb+=4*(ys1-yb)/abs(ys1-yb);  xb+=12*(xs1-xb)/abs(xs1-xb);}
    else if(abs(xs1-xb) >  abs(ys1-yb))            {yb+=4*(ys1-yb)/abs(ys1-yb);  xb+=8*(xs1-xb)/abs(xs1-xb);}
    else if(abs(xs1-xb) == abs (ys1-yb))          {yb+=4*(ys1-yb)/abs(ys1-yb);  xb+=4*(xs1-xb)/abs(xs1-xb);}

    if(a==0)
	   {if(pow(B[1].x-xb,2)+pow(B[1].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=B[1].x+10;
	      yb=B[1].y-2;
	      break;}
	     if(pow(B[2].x-xb,2)+pow(B[2].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=B[2].x+10;
	      yb=B[2].y-2;
	      break;}
	      }
    else    {if(pow(A[1].x-xb,2)+pow(A[1].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=A[1].x+10;
	      yb=A[1].y-2;
	      break;}
	     if(pow(A[2].x-xb,2)+pow(A[2].y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOAL
	     {xb=A[2].x+10;
	      yb=A[2].y-2;
	      break;}
	      }



    setfillstyle(1,2);
    bar(C.x-9,C.y-17,C.x+9,C.y);
    if(xb>C.x) C.x+=2;
    else if(xb<C.x) C.x-=2;
    setfillstyle(1,6);
    playerbody(C.x,C.y);
    delay(60);
    pieslice(xb,yb,0,360,2);
    if(yb<10 || yb>465)//CONDITION  WHEN BALL HAS REACHED THE GOAL
	 {settextstyle(4,0,5);
	  outtextxy(200,200,"GOAL GOAL GOAL!!");
	  if(yb<10)
	       {goal1++;yb+=20;}
	  if(yb>465)
	       {goal2++;yb-=20;}
	  delay(1000);
	  //necessary comments for goal
	  restriction();
	  break;


    }
    if(pow(C.x-xb,2)+pow(C.y-yb,2)<=100)//CONDITION WHEN THE BALL HAS REACHED THE GOALKEEPER
	  {xb=C.x+10;
	   yb=C.y-2;
	   break;}
delay(20);
}//for loop
pieslice(xb,yb,0,360,2);
}

void instruction()
{
cleardevice();
setbkcolor(1);
outtextxy(222,0,"INSTRUCTIONS");
outtextxy(50,50-5,"W        -   MOVE UP");
outtextxy(50,100-10,"S        -   MOVE DOWN");
outtextxy(50,150-15,"A        -   MOVE LEFT");
outtextxy(50,200-20,"D        -   MOVE RIGHT");
outtextxy(50,250-25,"I        -   PLAYER SWITCH");
outtextxy(50,300-30,"J        -   SHOOT");
outtextxy(50,350-35,"K        -   PASS");
outtextxy(50,400-40,"L        -   LONG BALL");
outtextxy(50,450-45,"Q        -   QUIT");
settextstyle(0,0,1);
}


void intro()
{
for(int yscr=350;yscr>=100;yscr--)
{for(int xscr=10;xscr<=210;xscr++)
	    {if(yscr>300&&yscr<350&&xscr>60&&xscr<160|| //lower part of J
	    yscr>150&&yscr<200||    //upper part of J
	    yscr>=200&&yscr<=300&&xscr>110&&xscr<160)   //vertical part of J
		      putpixel(xscr,yscr,1);
	     if(xscr<=60&&yscr<=250||xscr>110&&xscr<160&&yscr<=150)
		      putpixel(xscr,yscr,1);}
	    delay(10);
	    }
delay(240);
for(int xscr=210;xscr<=635;xscr++)
      {for(yscr=151;yscr<200;yscr++)
	     putpixel(xscr,yscr,1);
	     delay(3);
	     }


settextstyle(1,0,6);
setcolor(0);
outtextxy(245,140,"C");       delay(200);
outtextxy(290-8,140,"R");     delay(200);
outtextxy(340-10-8,140,"E");  delay(200);
outtextxy(390-15-18,140,"A"); delay(200);
outtextxy(440-20-28,140,"T"); delay(200);
outtextxy(490-25-35,140,"I"); delay(200);
outtextxy(540-30-57,140,"O"); delay(200);
outtextxy(590-35-65,140,"N"); delay(200);
outtextxy(640-40-70,140,"Z");
delay(1000);
settextstyle(2,0,3);
setcolor(15);
outtextxy(380,200,"P R E S E N T S");
delay(500);
getch();
cleardevice();
int p[134]={270,105,265,106,262,111,260,118,263,124,263,128,260,128,260,132,250,138,223,165,208,176,204,178,201,181,
	    204,189,206,186,206,190,213,184,218,180,253,155,258,163,240,197,233,203,225,215,200,238,198,243,200,248,
	    205,248,230,225,245,217,265,203,278,204,280,210,280,218,270,233,268,247,258,263,255,270,275,277,287,277,291,274,283,270,275,260,
	    300,210,300,200,292,172,291,140,305,127,304,125,327,103,337,99,339,96,335,98,338,92,335,94,338,89,332,92,334,88,333,87,325,92,322,98,302,115,278,128,277,125,280,119,280,110,276,106,270,105};
for(int i=0;i<134;i++)
      {p[i]*=2;
       if(i%2)
	   p[i]-=150;
       else p[i]-=375;}
setbkcolor(1);
setfillstyle(1,4);
fillpoly(67,p);
setfillstyle(1,1);
settextstyle(1,0,8);
setcolor(15);
delay(1000);
outtextxy(285,100,"STREET");
delay(1000);
outtextxy(250,200,"FOOTBALL");
delay(1000);
setfillstyle(1,4);
setcolor(4);
pieslice(100,350,0,360,20);
getch();
cleardevice();
setcolor(15);
setbkcolor(1);
setfillstyle(1,4);
fillpoly(67,p);
setfillstyle(1,4);
setcolor(4);
pieslice(100,350,0,360,20);
setcolor(15);
rectangle(295,105,490,190);
outtextxy(342,100,"LAY");
rectangle(250,250,560,310);
settextstyle(1,0,5);
outtextxy(277,250,"NSTRUCTIONS");
settextstyle(1,0,8);
setcolor(4);
outtextxy(300,100,"P");
settextstyle(1,0,5);
outtextxy(268,250,"I");
char ch;
ch=getch();
if(ch=='i' || ch=='I')
{instruction();
getch();             }

}


void restart()
{
delay(100);
A[1].x=520;
A[1].y=335;
A[2].x=300;
A[2].y=335;
B[1].x=520;
B[1].y=90;
B[2].x=300;
B[2].y=90;
x=A[1].x;
y=A[1].y;
xs=A[2].x;
ys=A[2].y;
delay(25);
}

void commentaryperm()
{
//TEAM NAMES
settextstyle(1,0,1);
setcolor(4);
outtextxy(60,10,"TEAM A");
outtextxy(40,30,A[0].name);
outtextxy(40,50,A[1].name);
outtextxy(40,70,A[2].name);
setcolor(1);
outtextxy(60,340,"TEAM B");
outtextxy(40,360,B[0].name);
outtextxy(40,380,B[1].name);
outtextxy(40,400,B[2].name);

//TIME DISPLAY
setcolor(4);
outtextxy(5,225,"MIN:");
outtextxy(80,225,"SECOND:");
setcolor(15);
}

void commentarytemp(char action)//TO DISPLAY DETAILS
{
//TEAM DISPLAY 1
settextstyle(1,0,1);
setcolor(4);
int ystar;
for(int i=0;i<3;i++)
   if(x==A[i].x)
       {ystar=30+20*i;
       break;}
outtextxy(160,ystar,"*");
settextstyle(1,0,0);
setcolor(15);

//TEAM DISPLAY 2
settextstyle(1,0,1);
setcolor(1);
int distanceB0= sqrt(pow(B[0].x-xb,2)+pow(B[0].y-yb,2));
int distanceB1= sqrt(pow(B[1].x-xb,2)+pow(B[1].y-yb,2));
int distanceB2= sqrt(pow(B[2].x-xb,2)+pow(B[2].y-yb,2));
int kt;
if(distanceB1<distanceB2 && distanceB1<distanceB0)      kt=1;
else if(distanceB0<distanceB2 && distanceB0<distanceB1) kt=2;
else if(distanceB2<distanceB1 && distanceB2<distanceB0) kt=0;
for(int j=0;j<3;j++)
   if(kt==j)
       ystar=360+20*kt;
outtextxy(160,ystar,"*");
settextstyle(2,0,4);
setcolor(4);

if(action=='a'||action=='A'||action=='s'||action=='S'||action=='d'||action=='D'||action=='w'||action=='W')//NAVIGATION
      outtextxy(40,110,A[i].name);
      if(pow(y-yb,2)+pow(x-xb,2)<=400)
	      if(y<200)
	      outtextxy(50,140,"dribbles the ball towards the goal");
	      else outtextxy(50,140,"dribbles the ball");
      else
	      outtextxy(50,140,"moves towards the ball");
char goal11[10],goal22[10];
outtextxy(20,200,"TEAM A       -       TEAM B");
itoa(goal1,goal11,10);
itoa(goal2,goal22,10);
outtextxy(80,200,goal11);
outtextxy(130,200,goal22);

if(action=='k')
{outtextxy(20,200,"A wonderful pass by");
outtextxy(200,200,A[1].name);}


if(action=='l')
outtextxy(20,200,"The ball is cleared");


if(action=='j')
{outtextxy(20,200,"SHOOT! SHOOT! SHOOT!");
 if(yb==10)
 {outtextxy(20,200,"Whatte beauty!! Goaaal!");};
}


//TIME DISPLAY
settextstyle(1,0,1);
setcolor(1);
outtextxy(50,225,minute);
outtextxy(160,225,second);
settextstyle(1,0,0);
setcolor(15);
}


void streetsoccer()
{
int count=0;
char action;

intro();

clock_t start, end;
start = clock();

randomize();
while(1)
{
delay(50);

cleardevice();
count++;
end = clock();
int timeelapsed= (end - start) / (CLK_TCK);
int sec= timeelapsed%60;
int min= timeelapsed/60;
itoa(min,minute,10);
itoa(sec,second,10);
randomize();
setbkcolor(2);
//pitch
rectangle(200,10,635,465);//pitch

restriction();

line(360,10,370,0);//top goal post - left
line(460,10,470,0);//top goal post - right
line(370,0,470,0); //top goal post - crossbar
line(360,465,370,455);//bottom goal post - left
line(460,465,470,455);//bottom goal post - right
line(370,455,470,455);//bottom goal post - crossbar
rectangle(340,400,490,465);//D BOX bottom
rectangle(340,10,490,75);//D BOX top

//team1,player1,goalkeeper,x1=420,y1=435
setfillstyle(1,4);
playerbody(A[0].x,A[0].y);

//team1,player2,RF,x2=550,y2=350
setfillstyle(1,4);
playerbody(A[1].x,A[1].y);

//team1,player3,LF,x3=300,y3=335
setfillstyle(1,4);
playerbody(A[2].x,A[2].y);

		//team2,player4,goalkeeper,x1=420,y1=30
		setfillstyle(1,1);
		playerbody(B[0].x,B[0].y);

		//team2,player5,LF,x2=550,y3=90
		setfillstyle(1,1);
		playerbody(B[1].x,B[1].y);

		//team2,player6,RF,x3=300,y3=90
		setfillstyle(1,1);
		playerbody(B[2].x,B[2].y);

commentarytemp(action);
commentaryperm();

randomize();
goalkeeper(A[0]);
	      goalkeeper(B[0]);
	      int k;
	      int distanceB1= sqrt(pow(B[1].x-xb,2)+pow(B[1].y-yb,2));
	      int distanceB2= sqrt(pow(B[2].x-xb,2)+pow(B[2].y-yb,2));
	      if(distanceB1<distanceB2)   {i=1;k=2;}
	      else                        {i=2;k=1;}

	      if(pow(B[i].x-xb,2)+pow(B[i].y-yb,2)<=50)
		     {B[i].y++;
		      yb++;
		      if   (B[i].x<random(100)+360)
			      {B[i].x++; xb++;}
		      else    {B[i].x--; xb--;}
		      if(366<=B[i].y &&B[i].y<=370)
			    shoot1(463,A[0]);
			    randomize();
		      int passcondition1=sqrt(pow(B[i].x-A[1].x,2)+pow(B[i].y-A[1].y,2));
		      int passcondition2=sqrt(pow(B[i].x-A[2].x,2)+pow(B[i].y-A[2].y,2));
		      int randomxD=random(5);
		      int passcondition=passcondition1>passcondition2?passcondition2:passcondition1;
		      if(passcondition<25 && randomxD==3)
			      pass(B[k].x,B[k].y);
		      }
	       else
		      {if(xb>B[i].x) B[i].x+=2;
		       else if(xb<B[i].x) B[i].x-=2;
		       if(yb>B[i].y) B[i].y+=2;
		       else if(yb<B[i].y) B[i].y-=2;}


//ball,xb=425,yb=435
setfillstyle(1,7);
pieslice(xb,yb,0,360,2);
		if(pow(B[0].x-xb,2)+pow(B[0].y-yb,2)<=50)
		{restart();
		setfillstyle(1,4);
		playerbody(A[1].x,A[1].y);
		playerbody(A[2].x,A[2].y);
		playerbody(B[1].x,B[1].y);
		playerbody(B[2].x,B[2].y);
		pass(B[1].x,B[1].y);}

if(pow(A[0].x-xb,2)+pow(A[0].y-yb,2)<=50)
{restart();
playerbody(A[1].x,A[1].y);
playerbody(A[2].x,A[2].y);
setfillstyle(1,1);
playerbody(B[1].x,B[1].y);
playerbody(B[2].x,B[2].y);
pass(A[1].x,A[1].y);}
if(kbhit())

action=getch();

if (action=='q'|| action=='Q')//QUIT
      { break;
      }
if (action=='i'||action=='I' )//PLAYER CHANGE
       swap();

if(action=='a'||action=='A'||action=='s'||action=='S'||action=='d'||action=='D'||action=='w'||action=='W')//NAVIGATION
       for(i=0;i<3;i++)
	   if(A[i].x==x &&A[i].y==y)
	       navigation(i,action);

if((action=='k'|| action=='K') && abs(x-xb)<10 && abs(y-yb)<10)//PASSING
       pass();

if((action=='l'|| action=='L') && abs(x-xb)<10 && abs(y-yb)<10)//LONG BALL
	longball();

if((action=='j'||action=='J') && abs(x-xb)<10 && abs(y-yb)<10)//SHOOT
	 {shoot1(0,B[0]);}

action='y';

if(min==1)
{//quit menu
settextstyle(1,0,4);
setcolor(4);
outtextxy(300,200,"GAME OVER");
if(goal1>goal2)
       outtextxy(250,300,"PLAYER 1 WINS");
else if(goal2>goal1)
 outtextxy(250,300,"PLAYER 2 WINS");
else
outtextxy(250,300,"MATCH DRAWN!");
delay(10000);
break;
}
}//while block
}



void foot()
{
int gdriver = DETECT, gmode, errorcode;
initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
streetsoccer();
cleardevice();
}
void main()
{do{
intromain();
cleardevice();
break;
}while(1);
quit();
}
