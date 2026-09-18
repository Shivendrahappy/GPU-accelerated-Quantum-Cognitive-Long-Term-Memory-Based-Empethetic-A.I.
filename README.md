# GPU-accelerated-Quantum-Cognitive-Long-Term-Memory-Based-Empethetic-A.I.
Project thesis -Questions and solutions in relation to GPU accelerated Long term Memory A.I. chatbot ,whether Quantum cognitive model possible in practical model at this time ,all learning outcome and working on related model .
This is the blue print
1. Memory dictionary
        ↓
2. Memory collection
        ↓
3. Dynamic memory addition
        ↓
4. Persistent JSON storage
        ↓
5. Retrieval
        ↓
6. Relevance selection
        ↓
7. Conversation integration
        ↓
8. LLM integration
        ↓
9. Affective/emotional context
        ↓
10. Quantum-cognition-inspired component
        ↓
11. Integration
        ↓
12. Evaluation
        ↓
13. GPU experimentation/optimization

STEP1 - 1 Long Term memory
For long term memory we start with making dictionary 'create" as step 1 as memory 1


create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}

print(create)
     
{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}

STEP 2. For set of memories - here 2nd memory is added into a list as Memory 2


create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}
memories = [create]
print (memories)
     
[{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}]
STEP 3. Create is the 1st memory we have already . Now create a second memomy - memory2 About my TOEFL preparation
WE ARE CREATING SECOND MEMORY 

memory2 = {
    'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing',
    'timestamp': '13 Sep 2026',
    'topic': 'learning',
    'importance': 0.9,
    'context': 'TOEFL study'
}
print(memory2)
     
{'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing', 'timestamp': '13 Sep 2026', 'topic': 'learning', 'importance': 0.9, 'context': 'TOEFL study'}
STEP 4 . Put the both in a memory collection - memories= [ create,memory2 ]
We have tp write the full  codes for create and the memory2

create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}
memory2 = {
    'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing',
    'timestamp': '13 Sep 2026',
    'topic': 'learning',
    'importance': 0.9,
    'context': 'TOEFL study'
}
memories =[create,memory2]
print(memories)
     
[{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}, {'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing', 'timestamp': '13 Sep 2026', 'topic': 'learning', 'importance': 0.9, 'context': 'TOEFL study'}]




memories
   │
   ├── create
   │     └── Python learning preference
   │
   └── memory2
         └── TOEFL learning preference
STEP - 5 (a) We need to add new memory to the existing ones using .append()      . memories.append(memory3) (No need to write previous codes again



memory3 = {
    'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises',
    'timestamp': '15 Sep 2026',
    'topic': 'learning',
    'importance': 0.5,
    'context': 'creative writing study'
}

print(memory3)


memory3 = {
    'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises',
    'timestamp': '15 Sep 2026',
    'topic': 'learning',
    'importance': 0.5,
    'context': 'creative writing study'
}


memory3 = {
    'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises',
    'timestamp': '15 Sep 2026',
    'topic': 'learning',
    'importance': 0.5,
    'context': 'creative writing study'
}

print(memory3)
print(memory3)
Step 5(b) To avoid writing the previous codes we use .append()memories.append(memory3)
print(memories)

memories.append(memory3)
print(memories)
Step 6 Check for how many items we have by len()
Step 6 Check for how many items we have by len()


print(len(memories))
     
4
Check by wrting all three memories


memories = [create,memory2,memory3]
print(memories)
     
[{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}, {'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing', 'timestamp': '13 Sep 2026', 'topic': 'learning', 'importance': 0.9, 'context': 'TOEFL study'}, {'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises', 'timestamp': '15 Sep 2026', 'topic': 'learning', 'importance': 0.5, 'context': 'creative writing study'}]

print(len(memories))
     
3
Step 7 Import JASON

Step 7 Import JASON


import json
     
Step 8 Save memories list into jason file


import json

create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}

memory2 = {
    'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing',
    'timestamp': '13 Sep 2026',
    'topic': 'learning',
    'importance': 0.9,
    'context': 'TOEFL study'
}
memory3 = {
    'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises',
    'timestamp': '15 Sep 2026',
    'topic': 'learning',
    'importance': 0.5,
    'context': 'creative writing study'
}

memories = [create,memory2,memory3]
with open ('memories.json','w') as file:
    json.dump(memories, file, indent=4)
     Date- 17 -Sep- 2026 Step 9 As I restart my laptop in each sessions so we check for runtime issue , has previous codes stored or not.


import os
print(os.path.exists('memories.json'))
     
False
Flase means old memories.jason is no longer in Collab runetime. It needs to recreate it

Step 10 a Recreate the memories ,so we have to do import json again with all codes as it also does because previous memories won't defined because collab has restarted


import json

create = {
    'content': 'I prefer learning Python with small examples',
    'timestamp': '10 Sep 2026',
    'topic': 'learning',
    'importance': 0.8,
    'context': 'python study'
}

memory2 = {
    'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing',
    'timestamp': '13 Sep 2026',
    'topic': 'learning',
    'importance': 0.9,
    'context': 'TOEFL study'
}
memory3 = {
    'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises',
    'timestamp': '15 Sep 2026',
    'topic': 'learning',
    'importance': 0.5,
    'context': 'creative writing study'
}

memories = [create,memory2,memory3]
print(memories)

with open ('memories.json','w') as file:
    json.dump(memories, file, indent=4)
     [{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}, {'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing', 'timestamp': '13 Sep 2026', 'topic': 'learning', 'importance': 0.9, 'context': 'TOEFL study'}, {'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises', 'timestamp': '15 Sep 2026', 'topic': 'learning', 'importance': 0.5, 'context': 'creative writing study'}]
     with open('memories.json', 'w') as file:open('memories.json', 'w'): This tells the computer to create a new file named memories.json. The 'w' stands for write mode. If the file already exists, it completely clears it out so you can write fresh data. If it doesn't exist, it creates it.with ... as file: This is a safety feature in Python. It safely opens the file and assigns it the temporary nickname file. The best part is that it automatically closes the file for you when the code finishes, preventing memory leaks or file corruption.2. json.dump(memories, file, indent=4)json.dump(): This is the translation engine. Computers store active data in RAM in a specific format, but files on your hard drive need to be written as plain text. This function converts your Python data (like a list or a dictionary) into text.memories: This is the actual data you want to save.file: This tells the function where to send that converted text (into the file we just opened).indent=4: This is purely for human eyes. It tells Python to format the text nicely with tabs and line breaks. Without this, all your data would be squeezed into one giant, unreadable line. With it, you can open the file and easily read it yourself.

     Step 10,b. Verify for the file exists or not


import os
print(os.path.exists('memories.json'))
     
True
Step 11) Downloading the file to the computer


from google.colab import files
files.download('memories.json')
     
file downloaded in pdf but not supported as pdf can't read jason file

Step 12 Load the JSON


with open('memories.json','r') as file:
    loaded_memories = json.load(file)
print(loaded_memories)
     [{'content': 'I prefer learning Python with small examples', 'timestamp': '10 Sep 2026', 'topic': 'learning', 'importance': 0.8, 'context': 'python study'}, {'content': 'I prefer learning TOEFL with small sessions of grammar ,vocab ,exersises and voice shadowing', 'timestamp': '13 Sep 2026', 'topic': 'learning', 'importance': 0.9, 'context': 'TOEFL study'}, {'content': 'I prefer learning creative writing through reading novels and weekend wrting excercises', 'timestamp': '15 Sep 2026', 'topic': 'learning', 'importance': 0.5, 'context': 'creative writing study'}]
