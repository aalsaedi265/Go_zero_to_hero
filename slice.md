
/ arrays ca not change size but are mustable in go
  var arr [2]int
  arr[0]=45
  fmt.Println(arr)
  
  //... is used instead of number, to count how much should be in there
  arr2 := [...]int{8,0,3} // make an arr with spefied itmes

    //nested arr
  arr3 := [...][2]string{{"the hadnd", "shining diamon"}, {"Deadly Queen", "Notorious BIG"} }

  for _, i := range arr3 {
    for j, str := range i{
        fmt.Println(j, str)
    }
  }

   arr := [...]int{1,2,3,4,5,6,7} <= cap is 5

    // begins a one index including value at one
    // ending at 4th index excludig 4th value

    sliceArr := arr[1:4] <= cap is 4 the starting index is changed, every change to x: alteres cap

    // cap is the max limt of number the arr can have
    // cap is obtained at [x]int with x being the cap
    fmt.Println(sliceArr ,cap(sliceArr))


     arr := [...]int{1,2,3,4,5,6,7}
    // begins a one index including value at one
    // ending at 4th index excludig 4th value
    sliceArr := arr[1:4]
    fmt.Println(arr,sliceArr)
    sliceArr[0]=98
    arr[3]=3000
    fmt.Println(arr,sliceArr)
 
     //capacity increase by a factor by a mutiple of 2 when increaded
    arr := []string{}// allows adding indefeintly to this slice ( not arr) lack of specifcatoin


for loop
    for i:=0; i < 10; i++{
        arr = append(arr, "ZaWorldo")
        fmt.Println(arr,len(arr), cap(arr))// how cap increase by mult of 2
    }
  
      arr := make([][]int, 5,10) // specifes the length and capacity of a slice


spread 
  arr := []bool{}
    arr2 := []bool{true, false,false}
    arr = append(arr, arr2...) // ... works like *arr in py, spread
 
   