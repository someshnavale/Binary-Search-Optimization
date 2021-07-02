# Binary-Search-Optimization


int array[1000] = { sorted list of numbers };
int N = 100; // number of entries in search space;
int high, low, mid; // our temporaries
int x; // value to search for
low = 0;
high = N -1;
while(low < high)
{
 mid = (low + high)/2;
 if(array[mid] < x)
 low = mid + 1;
 else
 high = mid;
}
if(array[low] == x)
 // found, index is low
else
 // not found
