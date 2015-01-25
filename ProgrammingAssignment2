
##This second programming assignment requires writing an R
##function that is able to cache potentially time-consuming computations.

##makevector is a special "vector" which is really a list containing a 
##a function to:
##1. Set the value of the vector
##2. Get the value of the vector
##3. Set the value of the mean
##4. Get the value of the mean
makeVector <- function(x = numeric()) {
  m <- NULL
  set <- function(y) {
    x <<- y
    m <<- NULL
  }
  get <- function() x
  setmean <- function(mean) m <<- mean
  getmean <- function() m
  list(set = set, get = get,
       setmean = setmean,
       getmean = getmean)
}
##The following function calculates the mean of the special "vector" 
##created with the above function. However, it first checks to see if 
##the mean has already been calculated. If so, it gets the mean from the 
##cache and skips the computation. Otherwise, it calculates the mean of 
##the data and sets the value of the mean in the cache via the setmean 
##function.
cachemean <- function(x, ...) {
  mm <- x$getmean()
  if(!is.null(m)) {
    message("getting cached data")
    return(m)
  }
  data <- x$get()
  m <- mean(data, ...)
  x$setmean(m)
  m
}
##makeCacheMatrix: This function creates a special "matrix" object 
##that can cache its inverse.
makeCacheMatrix <- function(x = matrix()) {
x<-makeCacheMatrix(mymatrix)  
}


##cacheSolve: This function computes the inverse of the special "matrix" 
##returned by makeCacheMatrix above. If the inverse has already been 
##calculated (and the matrix has not changed), then the cachesolve 
##should retrieve the inverse from the cache.

cacheSolve <- function(x, ...)  {
  CasheSolve(x)
        ## Return a matrix that is the inverse of 'x'
}

