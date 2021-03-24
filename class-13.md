### Link Home:
[Home](README.md)

# Reading Notes Code 201: Day 13

### The Past, Present, and Future of Local Storage for Web Applications

http://diveinto.html5doctor.com/storage.html 

Web cookies have been around since the very early days of the internet -- who knew! (They store very small amounts of data, only 4kb!). Cookie data also transmits to the server, so it's not always secure.

Microsoft's early `userData` allowed 64kb of storage per website domain.

Macromedia Flash introduced *Local Shares Objects* which allowed 100kb per domain. A later iteration of this creation allowed for relatively quick access of the Local Shared Objects via JavaScript.

Google's Gears allowed for infinite storage via a connected SQL database. 

All of the above depended on third party plugins.

#### HTML5 Storage

We might recognize it more as DOM storage. 

HTML5 storage is "...a way for web pages to store named key/value pairs locally, *within the client web browser*."

> -Source: http://diveinto.html5doctor.com/storage.html , emphasis mine

With HTML5 storage, your data exists if you close the website, but differs from cookies in that the data isn't transmitted to any server.

Access HTML5 storage through JavaScript with `localStorage`. **The data stored will be a string by default.** If you want it stored as some other data type, you will have to make that change yourself.

#### Why This is Useful

If you are playing a game in your browser and exit mid-way through playing, all your data will be erased if you go back to the site. With HTML5 storage, your last move(s) are saved "locally" (within the browser itself). Really, really cool stuff.

This section is incredible enough to include verbatim:

> [This function] uses the localStorage object to save whether there is a game in progress (gGameInProgress, a Boolean). If so, it iterates through the pieces (gPieces, a JavaScript Array) and saves the row and column number of each piece. Then it saves some additional game state, including which piece is selected (gSelectedPieceIndex, an integer), whether the piece is in the middle of a potentially long series of hops (gSelectedPieceHasMoved, a Boolean), and the total number of moves made so far (gMoveCount, an integer). 
>
> -Source: http://diveinto.html5doctor.com/storage.html

When the page loads (or reloads, in this case), rather than calling `newGame()`, `resumeGame()` is called instead. `resumeGame()` checks if there's already a game being played, and if there is, restores the values of that previous game.

--- 

HTML5 is currently in a great place, but the future is uncertain due to lots of competition (there are many versions of SQL).

**IndexedDB** is worth keeping an eye on.