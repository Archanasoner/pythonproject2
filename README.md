# pythonproject2
# count the no of words
# Import the required modules
import re


def count_words(input_text):
    input_text = input_text.strip()


    if not input_text:
        return 0


    words = re.findall(r'\b\w+\b', input_text)


    return len(words)

# Main function
def main():

    input_text = input("Please enter a sentence or paragraph: ")


    word_count = count_words(input_text)


    print("Word count:", word_count)


if __name__ == "__main__":
    main()
