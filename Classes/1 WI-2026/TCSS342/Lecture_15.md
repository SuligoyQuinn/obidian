# LZ77 Data Compression
- Maintains a window that slides along $T$, divided into two regions (past and future) by a thin line (present)
- The longest prefix of the future that occurs somewhere in the past is replaced by a pair (distance, length)
	- distance: number of characters to go back from present into the past
	- length: number of matching characters