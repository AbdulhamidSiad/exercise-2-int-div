# exercise-2-int-div
// See https://aka.ms/new-console-template for more information

//varibles for my code
int i20Packs = 0;
int i5Packs = 0;
int iSinglePack = 0;
int iUserInfo = 0;
int i20Remain = 0;
int i5Remain = 0;
int iSingleRemain = 0;
double dTotalCost = 0.0;
double d20Cost = 0.0;
double d5Cost = 0.0;
double dSingleCost = 0.0;




string sTitle = "Ticket Purchase";
Console.CursorLeft = (Console.WindowWidth - sTitle.Length) / 2;
Console.WriteLine(sTitle);
Console.Write("Enter the number of tickers to purchase:");
iUserInfo=int.Parse(Console.ReadLine());


//math
i20Packs = iUserInfo / 20;
i20Remain = iUserInfo % 20;
i5Packs = i20Remain / 5;
i5Remain = i20Remain % 5;
iSinglePack = i5Remain / 1;
iSingleRemain = i5Remain % 1;
d20Cost = i20Packs * 100.00;
d5Cost = i5Packs * 30.00;
dSingleCost = iSinglePack * 7.25;
dTotalCost = d20Cost + d5Cost + dSingleCost;

//display

Console.WriteLine("\nYou must purchase 5 20-pack<s>, 1 5-pack<s>, and 2 single tickets.\n");

Console.WriteLine($"The total cost is {dTotalCost:C2}\n");
Console.WriteLine("Press any key to continue:");





Console.ReadKey();
