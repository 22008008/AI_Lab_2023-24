# AI_Lab_2023-24
LAB EXPERIMENTS 
REQUIREMENTS 
1. PYHTON
2. SWI-PROLOG
3. PDDL 0R PDDL EDITOR ONLINE
4. JUPITER OR COLAB NOTEBOOK 

PROGRAM: 
graph = {
    '5': ['3', '7'],
    '3': ['2', '4'],
    '7': ['8'],
    '2': [],
    '4': ['8'],
    '8': []
}

visited = []  # List for visited nodes.
queue = []  # Initialize a queue

def bfs(visited, graph, node):  # Function for BFS
    visited.append(node)
    queue.append(node)
    
    while queue:  # Creating loop to visit each node
        m = queue.pop(0) 
        print(m) 
        
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)

# Driver Code
print("Following is the Breadth-First Search")
bfs(visited, graph, '5')

OUTPUT:

![image](https://github.com/user-attachments/assets/6ad485d6-0c45-4276-826f-c6b0b5729fc5)
