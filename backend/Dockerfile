FROM golang:1.19

# Set the working directory in the container
WORKDIR /app

# Copy the go.mod and go.sum files to the container
COPY go.mod go.sum ./

# Download the dependencies specified in the go.mod file
RUN go mod download

# Copy the entire project into the container
COPY . .

# Build the application
RUN go build -o main .

# Set the port that the backend listens on
EXPOSE 8080

# Run the application
CMD ["./main"]

