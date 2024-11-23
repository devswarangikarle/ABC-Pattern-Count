# ABC-Pattern-Count

Jake has a fascination with patterns in text. He has a string s of length n, made up of uppercase English letters, and he’s particularly interested in the pattern “ABC”. He wants to find out how many times this exact sequence appears as a continuous subsequences within s. Can you help Jake count these occurrences?

def count_abc_occurrences(n, s):

    count = 0
    for i in range(n - 2):  # Traverse up to index n-3
        if s[i:i + 3] == "ABC":
            count += 1
    return count

# Input
n = int(input().strip())
s = input().strip()

# Output
print(count_abc_occurrences(n, s))
