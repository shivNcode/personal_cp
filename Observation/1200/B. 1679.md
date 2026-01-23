https://codeforces.com/problemset/problem/1679/B

Obseravtion:
it was taking o(n) to implement the update array each time query 2 but i think if you use a global array of pair(value , lastupdate) and complary with a global pair(current value , lastupdate) so the things can be done in just o(1).