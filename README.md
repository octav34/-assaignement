NZIZA AIME OCTAVE
D/BBIT/21/01/13541


SUBMAIN()


        Dim size As Integer
        Console.Write("how many student you consider")
        size = Console.ReadLine()
        Dim student As String() = New String(size) {}
        Dim oop As Decimal() = New Decimal(size) {}
        Dim java As Decimal() = New Decimal(size) {}
        Dim c As Decimal() = New Decimal(size) {}
        Dim suma, sumb, sumc As Decimal
        Dim summ As Decimal
        suma = 0
        sumb = 0
        sumc = 0
        summ = 0
        For i As Integer = 0 To size - 1
            Console.Write("student" & i + 1 & ":")
            student(i) = Console.ReadLine()
            Console.WriteLine("marks for oop" & i + 1 & ":")
            oop(i) = Console.ReadLine()
            Console.WriteLine("marks for java" & i + 1 & ":")
            java(i) = Console.ReadLine()
            Console.WriteLine("marks for c" & i + 1 & ":")
            c(i) = Console.ReadLine()
            suma = (suma + oop(i))
            sumb = (sumb + java(i))
            sumc = (sumc + c(i))
            summ = (summ + oop(i) + java(i) + c(i))


        Next
        Console.WriteLine(" name |   OOp   | java    |   C  | ")
        For i As Integer = 0 To size - 1
            Console.WriteLine(student(i) & "" & oop(i) & "" & java(i) & "" & c(i))

        Next
        Console.ReadLine()


