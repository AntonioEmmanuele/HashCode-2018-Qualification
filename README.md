# HashCode-2020-Qualification
Solved with a greedy:

Algo:

remaining_time=deadline

score=0
Lk=[]
remaining_libs=libs
loop_value,loop_best_value,best_lib=0,-1,0 
while argminsub(libsSignupTime of remaining_libs)>remaining_time: 
	for lib in remaining_libs:
		if libsSignupTime[lib]>remaining_time
			remove(remaining_libs,lib)
		else 
			loop_value,NumBooks=calcScore(booksPerLibrary[lib],signupTime[lib],throughputs[lib],booksScore,deadline,remaining_timeLk)
			if loop_value>loop_best_value:
				loop_best_value=loop_value
				best_lib=lib 
	if loop_best_value==0:
		break
	remove(remaining_lib, best_lib)
            removed=0
	for book in booksPerLib[best_lib]:  #also the calculation is different
		if not book in Lk:
			append(Lk,book)
			score+=booksScore[books]
			removed++
		if removed==MaxBooks:
			break
	remaining_time-=signupTime[best_lib]


