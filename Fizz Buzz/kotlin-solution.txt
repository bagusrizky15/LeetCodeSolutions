class Solution {
    fun fizzBuzz(n: Int): List<String> {
        val total = mutableListOf<String>()
        for(i in 1..n){
            val mod3 = i%3
            val mod5 = i%5
            
            var hasil = ""
            if(mod3 ==0) hasil +="Fizz"
            if(mod5 ==0) hasil +="Buzz"
            if(hasil.isEmpty()) hasil += i.toString()
            
            total.add(hasil)
        }
        
        return total
    }
}  
