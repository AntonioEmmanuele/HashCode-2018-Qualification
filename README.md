# HashCode-2020-Qualification
Solved with a greedy:

Algo:

remaining_time=deadline

score=0 <br/>
Lk=[]<br/>
remaining_libs=libs<br/>
loop_value,loop_best_value,best_lib=0,-1,0<br/>
while argminsub(libsSignupTime of remaining_libs)>remaining_time:<br/>
	for lib in remaining_libs:<br/>
		if libsSignupTime[lib]>remaining_time<br/>
			remove(remaining_libs,lib)<br/>
		else <br/>
			loop_value,NumBooks=calcScore(booksPerLibrary[lib],signupTime[lib],throughputs[lib],booksScore,deadline,remaining_timeLk) <br/>
			if loop_value>loop_best_value:  <br/>
				loop_best_value=loop_value <br/>
				best_lib=lib <br/>
	if loop_best_value==0:<br/>
		break
	remove(remaining_lib, best_lib)<br/>
            removed=0 <br/>
	for book in booksPerLib[best_lib]:  #also the calculation is different <br/>
		if not book in Lk:  <br/>
			append(Lk,book)<br/>
			score+=booksScore[books]<br/>
			removed++ <br/>
		if removed==MaxBooks:<br/>
			break<br/>
	remaining_time-=signupTime[best_lib] <br/>


