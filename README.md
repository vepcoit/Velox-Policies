const xhr = new XMLHttpRequest();
    const url = "https://github.com/vepcoit/Velox-Policies"
    // Replace -username- with your GitHub username, -repo- with the repository name, and then :path with a path to the file or folder you want to get the content of (leave blank to ge all files of the repository)

    xhr.open('GET', URL, true);

    xhr.onload = function() {
        const data = JSON.parse(this.response);

        console.log(data);
    };
    
    xhr.send();
