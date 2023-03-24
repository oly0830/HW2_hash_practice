# HW2_hash_practice
with open('hw2_data.txt', 'r') as a:
    
    char_counts = {}

    for line in a:
        line = line.strip()
        if line in char_counts:
            char_counts[line] += 1
        
        else:
            char_counts[line] = 1

  
    num_unique_chars = len(char_counts)

   
    for char, count in char_counts.items():
        print(char, count)
