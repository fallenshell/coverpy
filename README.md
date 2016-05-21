# coverpy
Small wrapper for the iTunes API; mostly for fetching album covers. **Will soon be transferred over to Mxious, as it was built for it.** 

**Docs need to be done, I know. Been busy.**

## Install
This library requires Python 3.0+. It might work, but proceed with caution.
`pip install coverpy`
For development installs:
`make install`

## Testing
`make test`
Will run unit and coverage tests.

## Usage
Usage is very simple:
  
    # Instance CoverPy
    coverpy = coverpy.CoverPy()
    # Set a limit. There is a default (1), but I set it manually to showcase usage.
    limit = 1
    # Get results. Returns a Result object.
    result = coverpy.get_cover("OK Computer", limit)
    
    # Set a size for the artwork (first parameter) and get the result url.
    print result.artwork(100)
