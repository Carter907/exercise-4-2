```
BEGIN
	CLASS Program
		Main METHOD
			Console.WriteLine("salesperson: ");
			var salesperson = Console.ReadLine();
			var highestSale = 0;
			var highest = "";
			var grandTotal = 0;
			while (salesperson != "Z") {
				Console.WriteLine("sale: ");
				var sale = Convert.ToInt32(Console.ReadLine());
				grandTotal+=sale;
				if (sale > highestSale) {
					highest = salesperson;
					highestSale = sale;
				}
				Console.WriteLine("salesperson: ");
				salesperson = Console.ReadLine();
			}
			Console.WriteLine("Grand Total: ${0}", grandTotal);
			Console.WriteLine("Highest Sale: {0}", highest);		
		END Main
	END Program
END
```
