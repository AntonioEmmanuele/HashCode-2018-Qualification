# HashCode-2020-Qualification
Solved with a greedy:

Algo:

Until there is time for another lib: <br/>
> Select the lib with best Value <br/>
      Actual Time+=Best Value signup <br/>
      Update score with the books not yet sended or scheduled by previous libs <br/>
      
The value of a lib,at a time T, is calculated with a  ratio: <br/>
Numerator: Sum of the best books score, limited to the number of books that can be sended <br/>
Denominator: Library Signup time <br/>

Number Of Books=lib_throuput*(deadline-(T+signup Time))<br/>
The sumin the Numerator is limited to the books not already sended or scheduled to be sended by previously chosen libs<br/>
