def read_file(file_path):
    with open(file_path, 'r') as file:
        content = file.read()
        print(content)

def write_file(file_path, content):
    with open(file_path, 'w') as file:
        file.write(content)

def delete_file(file_path):
    os.remove(file_path)

# Example usage
file_name = input("Enter the file name: ")
user_content = input("Enter the content to write in the file: ")

write_file(file_name, user_content)
read_file(file_name)
delete_file(file_name)
