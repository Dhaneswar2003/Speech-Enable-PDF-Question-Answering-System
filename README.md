# Speech-Enable-PDF-Question-Answering-System

Text Processing Functions:

get_pdf_text(pdf_docs): This function extracts text from PDF documents uploaded by the user. get_text_chunks(text): This function splits the extracted text into smaller chunks. Language Processing and Embeddings:

get_vectorstore(text_chunks): This function creates a vector store using Hugging Face embeddings from the text chunks. Conversation Chain Setup:

get_conversation_chain(vectorstore): This function sets up a conversational retrieval chain using a language model and the vector store. User Interaction:

handle_userinput(user_question): This function handles user input (either text or speech) and provides a response using the conversational chain. Speech Input and Output:

speak(audio): This function takes an audio input and converts it to speech output using the pyttsx3 library. voiceinput(): This function listens to the user's voice input, recognizes it using Google's Speech Recognition API, and returns the recognized text. Streamlit App:

main(): This is the main function where the Streamlit app is defined. It sets up the user interface, including text input, file uploading, and buttons for interaction. File Uploading and Processing:

The Streamlit app allows users to upload PDF documents, process them, and then extract text for further analysis. Voice Interaction:

Users have the option to input their queries via voice by clicking the "Start" button, which triggers the voiceinput() function to capture their speech input. Overall, the code seems to be a combination of text processing, language processing, and user interface setup for a conversational retrieval system, with additional support for voice input and output.
