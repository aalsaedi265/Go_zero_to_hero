
     for i := 0; i < 10; i++{
        fmt.Println(i)
    }

     for x < 10 {  while loop
    x++
    fmt.Println(x)
   }

    jouskai :="Shining Diamond"

   for i:=0; i< len(jouskai); i++ {  // i or any verable its an int not a float64

    fmt.Println(jouskai[i]) //print out all utf8 nums, which are the bits each letter & space
    fmt.Printf("%c\n", jouskai[i]) // the \n so it does not print all on one line
   }

jouskai :="Shining Diamond"

// rage use int32 data type
  for i, el := range jouskai {// range is enumerator  _ used as palce holder for novarable

    //wiout string i would print bite number amount and not character in jouskai
    fmt.Println(i, string(el)) // index, letter
  }
 