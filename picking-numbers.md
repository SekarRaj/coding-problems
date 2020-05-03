Picking Numbers

https://www.hackerrank.com/challenges/picking-numbers/problem


```java
    public static int pickingNumbers(List<Integer> a) {
        int[] numbers = new int[100];

        for(int num: a){
            numbers[num - 1]++;
        }

        int max = 0;
        for(int i = 0; i < 100; i++){
            if(numbers[i] !=0){
                max = Math.max(max, (numbers[i] + numbers[i+1]));
            }
        }

        return max;
    }
```