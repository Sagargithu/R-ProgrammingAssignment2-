# I AM REALLY CONFUSED HOW TO SUBMIT THE PEER GRADED ASSIGNMENT OF COURSERA AND EVEN I DON'T KNOW THAT WHEATHER I HAVE SUCCESSFULLY SUBMITTED IT OR NOT. 
# SO IF ANY ONE IS FACING ANY PROBLEM PLEASE LET ME KNOW.


# Put comments here that give an overall description of what your
# makeCacheMatrix: This function creates a special “matrix” object that can cache its inverse.
#cacheSolve: This function computes the inverse of the special “matrix” returned by makeCacheMatrix above
#these functions can be used to set and get the value of matrix and value of inverse.

makeCacheMatrix <- function(x = matrix()) {
    i <- NULL
  set <- function(y) {
          x <<- y
          i <<- NULL
  }
  get <- function() x
  setinverse <- function(inverse) i <<- inverse
  getinverse <- function() i
  list(set = set,
       get = get,
       setinverse = setinverse,
       getinverse = getinverse)
}

## This function computes the inverse of the special “matrix” 
#returned by makeCacheMatrix above. If the inverse has already
#been calculated (and the matrix has not changed), then cacheSolve 
#should retrieve the inverse from the cache.

cacheSolve <- function(x, ...) {
  i <- x$getinverse()
  if (!is.null(i)) {
          message("getting cached data")
          return(i)
  }
  data <- x$get()
  i <- solve(data, ...)
  x$setinverse(i)
  i
}
