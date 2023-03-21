SR = lambda s, r, q : (q and not r) or s
JK = lambda j, k, q : (q and not k) or (j and not q)
D  = lambda d, q, x : d
T  = lambda t, q, x : (t and not q) or (not t and q)

if __name__ == "__main__":
	x = [int(item) for item in input('').split()]
	print("Qnext: " + str(D(x[0], x[1], x[2])))
