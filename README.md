# ArraySinifMethodlariOdevleri
[Kodluyoruz](https://app.patika.dev/) .Net eğitimi için hazırlanan C# Array Sınıfı Methodları ödevidir. HackerRank'ta çözülmüş 7 farklı sorunun cevabı için oluşturulmuştur.
## HackerRank
- HackerRank problemlerinde kod yazılan kısımlar eklenmiştir.
### Birthday Cake Candles
```
   public static int birthdayCakeCandles(List<int> candles)
    {
        int count = 0;
        int max = 0;
        foreach (var candle in candles)
        {
            int num = candle;
            if(num > max)
        {
            max = num;
            count = 1;
        }
        else if(max == num)
        {
            count++;
        }
    }
    return count;

    }
```
## Simple Array Sum
```
    public static int simpleArraySum(List<int> ar)
    {
        int sum = 0;
        foreach( var item in ar)
        {
            sum += item;
        }
        return sum;

    }
```
## Day 7: Arrays
```
        List<int> arr = Console.ReadLine().TrimEnd().Split(' ').ToList().Select(arrTemp 
        => Convert.ToInt32(arrTemp)).ToList();
        
        ReversePrint(arr);
    }
    
    private static void ReversePrint(List<int>arr)
    {
        int length = arr.Count;
        
        for(int i = length - 1; i >=0; i--)
        {
            if(i != 0)
            {
                Console.Write(arr[i] + " ");
            }
            else
            {
                Console.Write(arr[i]);
            }
        }
    }
        
}
```
## A Very Big Sum
```
    public static long aVeryBigSum(List<long> ar)
    {
        long sum = ar.Sum();
        return sum;
    }
```
## Compare the Triplets
```
    public static List<int> compareTriplets(List<int> a, List<int> b)
    {
        List<int> scores = new List<int>() {0, 0 };
        for (int i =0; i < a.Count; i++)
        {
            if(a[i] > b[i]) scores[0]++;
            else if(a[i] < b[i]) scores[1]++; 
        }
        return scores;

    }
```
## Day 20: Sorting
```
        List<int> a = Console.ReadLine().TrimEnd().Split(' ').ToList().Select(aTemp 
        => Convert.ToInt32(aTemp)).ToList();
        
        BubbleSort(a);
    }
    
    public static void BubbleSort(List<int> list)
    {
        var numberOfSwaps = 0;
        for(var i = 0; i < list.Count; i++)
        {
            for(var j = 0; j < list.Count - 1; j++)
            {
                if(list[j] > list[j + 1])
                {
                    var temp = list[j];
                    list[j] = list[j +1];
                    list[j + 1] = temp;
                    numberOfSwaps++;
                }
            }
            if (numberOfSwaps == 0) 
            {
                break;
            }
        }
        Console.WriteLine($"Array is sorted in {numberOfSwaps} swaps.");
        Console.WriteLine($"First Element: {list[0]}");
        Console.WriteLine($"Last Element: {list[list.Count - 1]}");
    }  
}
```
## Migratory Birds
```
 public static int migratoryBirds(List<int> arr)
    {
        int[] count = new int[arr.Max()];
        int max = 0, c = 0;
        for(int i=0; i<arr.Count; i++)
        {
            count[arr[i]-1]++;
        }
        for(int i=0; i<count.Length; i++)
        {
            if(max<count[i]) {max = count[i]; c = i; }
        }
        return c + 1;
    }
```
### [Hacker Rank Profilim](https://www.hackerrank.com/ogulcan_celik24) 
#### https://www.hackerrank.com/ogulcan_celik24
#### www.patika.dev