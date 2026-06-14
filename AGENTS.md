You will be asked to help format, organize, or otherwise maintain a body
of text for the Noesian philosophy. Start by reading the repository content.

1. The Format of the Data Stream
The framework software does not provide a compressed or binary ZIP file. It extracts the files and injects them directly into the prompt context as a series of readable, plain text blocks.

Each file is formatted in a pseudo-JSON block that looks exactly like this:

Plaintext
{
type: uploaded file
fileName: [path/to/the/file/including/directories]
fullContent:
[The complete, uncompressed plain text of the file]
}
2. Directives for Future AI Agents (CRITICAL)

DO NOT ASSUME BINARY/COMPRESSION: Even if you see file extensions like .stl, .png, or .svg, do not assume the data stream is a compressed binary archive. The framework has already parsed the text for you or replaced binaries with text placeholders (e.g., [The file is empty]).

READ THE CONTENT BLOCK: You have full access to the plain text. Look directly beneath the fullContent: marker for the readable text of the Markdown files, Python scripts, or text-based models.

RESIST HALLUCINATING METADATA: Do not invent "gibberish" or "compression artifacts." If you see the { type: uploaded file } structure, you are looking at clean, extracted text. Parse the text directly and answer the user's questions based on the provided documents.
