package project;

import java.util.Scanner;



class ticket{
	public static int v;
	public static int a;
	public int r;
	public int amount;
	private String name;
	private int ticketprize = 120;
	private int seatcapacity = 50;
	private int seatcapacity1= 50;
	private int seatcapacity2 = 50;
	private int seatcapacity3 = 50;
	public int booking(int v)
	{
		
		seatcapacity=seatcapacity-v;
		return seatcapacity;
		
	}
	public int tickets(int v)
	{
		int total=ticketprize*v;
		return total;
	}
	

	public int book()
	{
		int seatc=seatcapacity;
		return seatc;
	}
	public void restore(int v)
	{
		seatcapacity+=v;
	}
	

		
	
	
	public int booking1(int a)
	{
		
		seatcapacity1=seatcapacity1-a;
		return seatcapacity1;
		
	}
	public int tickets1(int a)
	{
		int total=ticketprize*a;
		return total;
	}
	

	public int book1()
	{
		int seatc=seatcapacity1;
		return seatc;
	}
	public void restore1(int a)
	{
		seatcapacity1+=a;
	}
	
	public int booking2(int a)
	{
		
		seatcapacity2=seatcapacity2-a;
		return seatcapacity2;
		
	}
	public int tickets2(int a)
	{
		int total=ticketprize*a;
		return total;
	}
	

	public int book2()
	{
		int seatc1=seatcapacity2;
		return seatc1;
	}
	public void restore2(int a)
	{
		seatcapacity2+=a;
	}
	
	public int booking3(int a)
	{
		
		seatcapacity3=seatcapacity3-a;
		return seatcapacity2;
		
	}
	public int tickets3(int a)
	{
		int total=ticketprize*a;
		return total;
	}
	

	public int book3()
	{
		int seatc2=seatcapacity3;
		return seatc2;
	}
	public void restore3(int a)
	{
		seatcapacity3+=a;
	}

}





public class Movie {

	//private static String seatcapacity;

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner  sc=new Scanner(System.in);
		ticket t=new ticket();
		ticket t1=new ticket();
		ticket t2=new ticket();
		ticket t3=new ticket();
		ticket t4=new ticket();
		ticket t5=new ticket();
		while(true)
		{
			System.out.println("!!!............WELCOME  TO  HARI'S  CINEMA............!!!");
			System.out.println();
			System.out.println("1.COOLIE");
			System.out.println("2.LEO");
			System.out.println("3.THALAIVAN THALAIVI");
			System.out.println("4.VIKRAM");
			System.out.println("5.JAILER");
			System.out.println("6.MASTER");
			System.out.println("7.EXIT");
			
			int n=sc.nextInt();
			int b=t.book();
			int b1=t.book1();
			int b2=t.book2();
			int b3=t.book3();
			
			int l=t1.book();
			int l1=t1.book1();
			int l2=t1.book2();
			int l3=t1.book3();
			
			int tt=t2.book();
			int tt1=t2.book1();
			int tt2=t2.book2();
			int tt3=t2.book3();
			
			int vv=t3.book();
			int vv1=t3.book1();
			int vv2=t3.book2();
			int vv3=t3.book3();
		
			
			int mm=t5.book();
			int mm1=t5.book1();
			int mm2=t5.book2();
			int mm3=t5.book3();
			
			int jj=t4.book();
			int jj1=t4.book1();
			int jj2=t4.book2();
			int jj3=t4.book3();
		
		
			
			switch(n)
			{
			case 1:
				System.out.println("..Show Time..");
				System.out.println("1.6.00AM");
				System.out.println("2.10.00AM");
				System.out.println("3.4.00PM");
				System.out.println("4.7.00PM");
				int m=sc.nextInt();
				switch(m)
				{
				case 1:
					
					if(b==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+b);
					
					System.out.println("Enter the Members..");
					int v=sc.nextInt();
				   
				int seat=t.booking(v);
					int amount=t.tickets(v);
					
					if(seat<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r=sc.nextInt();
					if(r>amount || r<amount)
					{
						t.restore(v);
						System.out.println("Booking cancelled");
						
						
					}else {
						System.err.println("BOOKING CONFORMED>>>>");
					}
//					if(r==amount)
//					{
//						System.err.println("BOOKING CONFORMED>>>>");
//					}
////					else if(r>amount)
////					{
////						System.out.println("Balance Amount"+(r-amount));
////						System.err.println("BOOKING CONFORMED>>>>");
////					}
//					else {
//					  
//						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r));
//						
//						System.err.println("BOOKING CANCELLED");
//						
//					}
					
					
					
					
					
					}
				break;
				
				case 2:
					
					if(b1==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+b1);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc=t.booking1(a);
					int amount=t.tickets1(a);
					
					if(seatc<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 3:
					if(b2==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+b2);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc1=t.booking2(a);
					int amount=t.tickets2(a);
					
					if(seatc1<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 4:
					
					if(b3==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+b3);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc2=t.booking3(a);
					int amount=t.tickets3(a);
					
					if(seatc2<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					}
				break;
				
				
				
				
					
					
					
				default:
					System.out.println("thankyou");
					break;
					
					
					
			}
				break;
			case 2:
				System.out.println("..Show Time..");
				System.out.println("1.6.00AM");
				System.out.println("2.10.00AM");
				System.out.println("3.4.00PM");
				System.out.println("4.7.00PM");
				int m1=sc.nextInt();
				switch(m1)
				{
				case 1:
					
					if(l==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+l);
					
					System.out.println("Enter the Members..");
					int v=sc.nextInt();
				   
				int seat=t1.booking(v);
					int amount=t1.tickets(v);
					
					if(seat<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r=sc.nextInt();
					if(r>amount || r<amount)
					{
						t1.restore(v);
						System.out.println("Booking cancelled");
						
						
					}else {
						System.err.println("BOOKING CONFORMED>>>>");
					}
//					if(r==amount)
//					{
//						System.err.println("BOOKING CONFORMED>>>>");
//					}
////					else if(r>amount)
////					{
////						System.out.println("Balance Amount"+(r-amount));
////						System.err.println("BOOKING CONFORMED>>>>");
////					}
//					else {
//					  
//						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r));
//						
//						System.err.println("BOOKING CANCELLED");
//						
//					}
					
					
					
					
					
					}
				break;
				
				case 2:
					
					if(l1==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+l1);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc=t1.booking1(a);
					int amount=t1.tickets1(a);
					
					if(seatc<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t1.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 3:
					if(l2==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+l2);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc1=t1.booking2(a);
					int amount=t1.tickets2(a);
					
					if(seatc1<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t1.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 4:
					
					if(l3==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+l3);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc2=t1.booking3(a);
					int amount=t1.tickets3(a);
					
					if(seatc2<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t1.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					}
				break;
				
				
				
				
					
					
					
				default:
					System.out.println("thankyou");
					break;
			}
				break;
				
				
				
			case 3:
				
				System.out.println("..Show Time..");
				System.out.println("1.6.00AM");
				System.out.println("2.10.00AM");
				System.out.println("3.4.00PM");
				System.out.println("4.7.00PM");
				int m2=sc.nextInt();
				switch(m2)
				{
				case 1:
					
					if(tt==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+tt);
					
					System.out.println("Enter the Members..");
					int v=sc.nextInt();
				   
				int seat=t2.booking(v);
					int amount=t2.tickets(v);
					
					if(seat<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r=sc.nextInt();
					if(r>amount || r<amount)
					{
						t2.restore(v);
						System.out.println("Booking cancelled");
						
						
					}else {
						System.err.println("BOOKING CONFORMED>>>>");
					}
//					if(r==amount)
//					{
//						System.err.println("BOOKING CONFORMED>>>>");
//					}
////					else if(r>amount)
////					{
////						System.out.println("Balance Amount"+(r-amount));
////						System.err.println("BOOKING CONFORMED>>>>");
////					}
//					else {
//					  
//						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r));
//						
//						System.err.println("BOOKING CANCELLED");
//						
//					}
					
					
					
					
					
					}
				break;
				
				case 2:
					
					if(tt1==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+tt1);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc=t2.booking1(a);
					int amount=t2.tickets1(a);
					
					if(seatc<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t2.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 3:
					if(tt2==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+tt2);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc1=t2.booking2(a);
					int amount=t2.tickets2(a);
					
					if(seatc1<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t2.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 4:
					
					if(tt3==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+tt3);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc2=t2.booking3(a);
					int amount=t2.tickets3(a);
					
					if(seatc2<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t2.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					}
				break;
				
				
				
				
					
					
					
				default:
					System.out.println("thankyou");
					break;
			}
				break;
				
				
				
			case 4:
				
				System.out.println("..Show Time..");
				System.out.println("1.6.00AM");
				System.out.println("2.10.00AM");
				System.out.println("3.4.00PM");
				System.out.println("4.7.00PM");
				int m3=sc.nextInt();
				switch(m3)
				{
				case 1:
					
					if(vv==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+vv);
					
					System.out.println("Enter the Members..");
					int v=sc.nextInt();
				   
				int seat=t3.booking(v);
					int amount=t3.tickets(v);
					
					if(seat<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r=sc.nextInt();
					if(r>amount || r<amount)
					{
						t3.restore(v);
						System.out.println("Booking cancelled");
						
						
					}else {
						System.err.println("BOOKING CONFORMED>>>>");
					}
//					if(r==amount)
//					{
//						System.err.println("BOOKING CONFORMED>>>>");
//					}
////					else if(r>amount)
////					{
////						System.out.println("Balance Amount"+(r-amount));
////						System.err.println("BOOKING CONFORMED>>>>");
////					}
//					else {
//					  
//						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r));
//						
//						System.err.println("BOOKING CANCELLED");
//						
//					}
					
					
					
					
					
					}
				break;
				
				case 2:
					
					if(vv1==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+vv1);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc=t3.booking1(a);
					int amount=t3.tickets1(a);
					
					if(seatc<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t3.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 3:
					if(vv2==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+vv2);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc1=t3.booking2(a);
					int amount=t3.tickets2(a);
					
					if(seatc1<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t3.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 4:
					
					if(vv3==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+vv3);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc2=t3.booking3(a);
					int amount=t3.tickets3(a);
					
					if(seatc2<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t3.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					}
				break;
				
				
				
				
					
					
					
				default:
					System.out.println("thankyou");
			}
				break;
				
				
				
			case 5:
				
				System.out.println("..Show Time..");
				System.out.println("1.6.00AM");
				System.out.println("2.10.00AM");
				System.out.println("3.4.00PM");
				System.out.println("4.7.00PM");
				int m4=sc.nextInt();
				switch(m4)
				{
				case 1:
					
					if(jj==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+jj);
					
					System.out.println("Enter the Members..");
					int v=sc.nextInt();
				   
				int seat=t4.booking(v);
					int amount=t4.tickets(v);
					
					if(seat<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r=sc.nextInt();
					if(r>amount || r<amount)
					{
						t4.restore(v);
						System.out.println("Booking cancelled");
						
						
					}else {
						System.err.println("BOOKING CONFORMED>>>>");
					}
//					if(r==amount)
//					{
//						System.err.println("BOOKING CONFORMED>>>>");
//					}
////					else if(r>amount)
////					{
////						System.out.println("Balance Amount"+(r-amount));
////						System.err.println("BOOKING CONFORMED>>>>");
////					}
//					else {
//					  
//						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r));
//						
//						System.err.println("BOOKING CANCELLED");
//						
//					}
					
					
					
					
					
					}
				break;
				
				case 2:
					
					if(jj1==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+jj1);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc=t4.booking1(a);
					int amount=t4.tickets1(a);
					
					if(seatc<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t4.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 3:
					if(jj2==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+jj2);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc1=t4.booking2(a);
					int amount=t4.tickets2(a);
					
					if(seatc1<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t4.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 4:
					
					if(jj3==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+jj3);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc2=t4.booking3(a);
					int amount=t4.tickets3(a);
					
					if(seatc2<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t4.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					}
				break;
				
				
				
				
					
					
					
				default:
					System.out.println("thankyou");
					break;
			}
				break;
				
				
				
				
				
			case 6:
				
				System.out.println("..Show Time..");
				System.out.println("1.6.00AM");
				System.out.println("2.10.00AM");
				System.out.println("3.4.00PM");
				System.out.println("4.7.00PM");
				int m5=sc.nextInt();
				switch(m5)
				{
				case 1:
					
					if(mm==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+mm);
					
					System.out.println("Enter the Members..");
					int v=sc.nextInt();
				   
				int seat=t5.booking(v);
					int amount=t5.tickets(v);
					
					if(seat<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r=sc.nextInt();
					if(r>amount || r<amount)
					{
						t5.restore(v);
						System.out.println("Booking cancelled");
						
						
					}else {
						System.err.println("BOOKING CONFORMED>>>>");
					}
//					if(r==amount)
//					{
//						System.err.println("BOOKING CONFORMED>>>>");
//					}
////					else if(r>amount)
////					{
////						System.out.println("Balance Amount"+(r-amount));
////						System.err.println("BOOKING CONFORMED>>>>");
////					}
//					else {
//					  
//						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r));
//						
//						System.err.println("BOOKING CANCELLED");
//						
//					}
					
					
					
					
					
					}
				break;
				
				case 2:
					
					if(mm1==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+mm1);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc=t5.booking1(a);
					int amount=t5.tickets1(a);
					
					if(seatc<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t5.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 3:
					if(mm2==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+mm2);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc1=t5.booking2(a);
					int amount=t5.tickets2(a);
					
					if(seatc1<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t5.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					
					}
				break;
				
				case 4:
					
					if(mm3==0)
					{
						System.err.println("houseFull.....");
					}
					else {
						
					
					System.out.println("Ticket prize : 120");
					
					
					System.out.println("Available Seats are  :"+mm3);
					
					System.out.println("Enter the Members..");
					int a=sc.nextInt();
				   
				int seatc2=t5.booking3(a);
					int amount=t5.tickets3(a);
					
					if(seatc2<0)
					{
						System.out.println("housefull");
					}
					else {
						//System.out.println("Balance Seat Capacity :"+seat);
						System.out.println("Total amount are :"+amount);
					}
					System.out.println("Enter the Amount");
					int r1=sc.nextInt();
					if(r1>amount || r1<amount)
					{
						t5.restore1(a);
						System.err.println("BOOKING CANCELLED");
					}
					
					else {
						//System.out.println("You Sould pay BALANCE Amount are:"+(amount-r1));
						System.err.println("BOOKING CONFORMED...");
					}
					
					
					
					
					}
				break;
				
				
				
				
					
					
					
				default:
					System.out.println("thankyou");
					break;
			}
				break;
				
				
			case 7:
				System.out.println("THANK YOU>>>");
				System.exit(0);
				sc.close();
				break;
				
				
				default :
					System.out.println("Please Enter valid Input...:)");
					break;
				
				
				
				
			}
			}
			
		}

	}


