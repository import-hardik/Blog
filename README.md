# Blog Website - HTML, CSS, JS, Express, MongoDB

This is a simple blog website built using HTML, CSS, and JavaScript for the frontend, and Express.js with MongoDB for the backend. The website allows users to view blog posts, and admin users can create, edit, and delete blog entries directly from the backend.

## Features

- **View Blogs**: Users can view a collection of blog posts with a clean interface.
- **Read Blog Details**: Each blog post has a detailed view displaying the full content.
- **Create, Edit, Delete Blogs**: Admins can manage blog content (create, edit, delete) via the backend API.
- **Responsive Design**: The website layout adjusts based on device size for optimal viewing on mobile, tablet, and desktop.
- **No Authentication**: This website is open to all users for reading blogs without login.

## Tech Stack

- **Frontend**:
  - **HTML5**: Structure of the website
  - **CSS3**: Styling and layout
  - **JavaScript**: Interactive client-side functionality
- **Backend**:
  - **Node.js & Express.js**: For building RESTful APIs
  - **MongoDB**: NoSQL database for storing blog data (with Mongoose for schema modeling)
- **Version Control**: Git, GitHub

## Installation and Setup

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/import-hardik/Blog.git
   ```

2. **Navigate into the project directory**:
   ```bash
   cd Blog
   ```

3. **Install backend dependencies**:
   ```bash
   cd backend
   npm install
   ```

4. **Configure environment variables**:  
   Create a `.env` file in the `backend` directory with the following:
   ```
   MONGO_URI=<Your MongoDB URI>
   ```

5. **Run the backend server**:
   ```bash
   npm start
   ```

6. **Open the frontend**:  
   Navigate to the `frontend` folder, and open the `index.html` file in a web browser.

The website should now be running on `http://localhost:5000` for backend APIs, while the frontend HTML/CSS/JS is directly served by your browser.

## Folder Structure

```
Blog
    └───Blogs
        ├───models
        ├───node_modules
        │   ├───.bin
        │   ├───@mongodb-js
        │   │   └───saslprep
        │   │       └───dist
        │   ├───@types
        │   │   ├───webidl-conversions
        │   │   └───whatwg-url
        │   │       └───lib
        │   ├───accepts
        │   ├───ansi-styles
        │   ├───anymatch
        │   ├───array-flatten
        │   ├───async
        │   │   ├───dist
        │   │   └───internal
        │   ├───balanced-match
        │   │   └───.github
        │   ├───binary-extensions
        │   ├───body-parser
        │   │   └───lib
        │   │       └───types
        │   ├───brace-expansion
        │   ├───braces
        │   │   └───lib
        │   ├───bson
        │   │   ├───etc
        │   │   ├───lib
        │   │   ├───src
        │   │   │   ├───parser
        │   │   │   │   └───on_demand
        │   │   │   └───utils
        │   │   └───vendor
        │   │       ├───base64
        │   │       └───text-encoding
        │   │           └───lib
        │   ├───bytes
        │   ├───call-bind
        │   │   ├───.github
        │   │   └───test
        │   ├───chalk
        │   │   └───source
        │   ├───chokidar
        │   │   ├───lib
        │   │   └───types
        │   ├───color-convert
        │   ├───color-name
        │   ├───concat-map
        │   │   ├───example
        │   │   └───test
        │   ├───content-disposition
        │   ├───content-type
        │   ├───cookie
        │   ├───cookie-signature
        │   ├───debug
        │   │   └───src
        │   ├───define-data-property
        │   │   ├───.github
        │   │   └───test
        │   ├───depd
        │   │   └───lib
        │   │       └───browser
        │   ├───destroy
        │   ├───ee-first
        │   ├───ejs
        │   │   ├───bin
        │   │   └───lib
        │   ├───encodeurl
        │   ├───es-define-property
        │   │   ├───.github
        │   │   └───test
        │   ├───es-errors
        │   │   ├───.github
        │   │   └───test
        │   ├───escape-html
        │   ├───etag
        │   ├───express
        │   │   └───lib
        │   │       ├───middleware
        │   │       └───router
        │   ├───filelist
        │   │   └───node_modules
        │   │       ├───brace-expansion
        │   │       │   └───.github
        │   │       └───minimatch
        │   │           └───lib
        │   ├───fill-range
        │   ├───finalhandler
        │   ├───forwarded
        │   ├───fresh
        │   ├───function-bind
        │   │   ├───.github
        │   │   └───test
        │   ├───get-intrinsic
        │   │   ├───.github
        │   │   └───test
        │   ├───glob-parent
        │   ├───gopd
        │   │   ├───.github
        │   │   └───test
        │   ├───has-flag
        │   ├───has-property-descriptors
        │   │   ├───.github
        │   │   └───test
        │   ├───has-proto
        │   │   ├───.github
        │   │   └───test
        │   ├───has-symbols
        │   │   ├───.github
        │   │   └───test
        │   │       └───shams
        │   ├───hasown
        │   │   └───.github
        │   ├───http-errors
        │   ├───iconv-lite
        │   │   ├───encodings
        │   │   │   └───tables
        │   │   └───lib
        │   ├───ignore-by-default
        │   ├───inherits
        │   ├───ipaddr.js
        │   │   └───lib
        │   ├───is-binary-path
        │   ├───is-extglob
        │   ├───is-glob
        │   ├───is-number
        │   ├───jake
        │   │   ├───bin
        │   │   ├───lib
        │   │   │   ├───task
        │   │   │   └───utils
        │   │   └───test
        │   │       ├───integration
        │   │       │   └───jakelib
        │   │       └───unit
        │   ├───kareem
        │   ├───media-typer
        │   ├───memory-pager
        │   ├───merge-descriptors
        │   ├───method-override
        │   │   └───node_modules
        │   │       └───debug
        │   │           └───src
        │   ├───methods
        │   ├───mime
        │   │   └───src
        │   ├───mime-db
        │   ├───mime-types
        │   ├───minimatch
        │   ├───mongodb
        │   │   ├───etc
        │   │   ├───lib
        │   │   │   ├───bulk
        │   │   │   ├───client-side-encryption
        │   │   │   │   └───providers
        │   │   │   ├───cmap
        │   │   │   │   ├───auth
        │   │   │   │   │   └───mongodb_oidc
        │   │   │   │   ├───handshake
        │   │   │   │   └───wire_protocol
        │   │   │   │       └───on_demand
        │   │   │   ├───cursor
        │   │   │   ├───gridfs
        │   │   │   ├───operations
        │   │   │   │   ├───client_bulk_write
        │   │   │   │   └───search_indexes
        │   │   │   └───sdam
        │   │   └───src
        │   │       ├───bulk
        │   │       ├───client-side-encryption
        │   │       │   └───providers
        │   │       ├───cmap
        │   │       │   ├───auth
        │   │       │   │   └───mongodb_oidc
        │   │       │   ├───handshake
        │   │       │   └───wire_protocol
        │   │       │       └───on_demand
        │   │       ├───cursor
        │   │       ├───gridfs
        │   │       ├───operations
        │   │       │   ├───client_bulk_write
        │   │       │   └───search_indexes
        │   │       └───sdam
        │   ├───mongodb-connection-string-url
        │   │   └───lib
        │   ├───mongoose
        │   │   ├───dist
        │   │   ├───lib
        │   │   │   ├───cast
        │   │   │   ├───cursor
        │   │   │   ├───drivers
        │   │   │   │   ├───browser
        │   │   │   │   └───node-mongodb-native
        │   │   │   ├───error
        │   │   │   ├───helpers
        │   │   │   │   ├───aggregate
        │   │   │   │   ├───cursor
        │   │   │   │   ├───discriminator
        │   │   │   │   ├───document
        │   │   │   │   ├───error
        │   │   │   │   ├───indexes
        │   │   │   │   ├───model
        │   │   │   │   ├───path
        │   │   │   │   ├───populate
        │   │   │   │   ├───projection
        │   │   │   │   ├───query
        │   │   │   │   ├───schema
        │   │   │   │   ├───schematype
        │   │   │   │   ├───timestamps
        │   │   │   │   ├───topology
        │   │   │   │   └───update
        │   │   │   ├───options
        │   │   │   ├───plugins
        │   │   │   ├───schema
        │   │   │   │   └───operators
        │   │   │   └───types
        │   │   │       ├───array
        │   │   │       │   └───methods
        │   │   │       └───documentArray
        │   │   │           └───methods
        │   │   ├───node_modules
        │   │   │   └───ms
        │   │   └───types
        │   ├───mpath
        │   │   ├───lib
        │   │   └───test
        │   ├───mquery
        │   │   ├───.github
        │   │   ├───lib
        │   │   │   └───collection
        │   │   └───node_modules
        │   │       ├───debug
        │   │       │   └───src
        │   │       └───ms
        │   ├───ms
        │   ├───negotiator
        │   │   └───lib
        │   ├───nodemon
        │   │   ├───bin
        │   │   ├───doc
        │   │   │   └───cli
        │   │   ├───lib
        │   │   │   ├───cli
        │   │   │   ├───config
        │   │   │   ├───help
        │   │   │   ├───monitor
        │   │   │   ├───rules
        │   │   │   └───utils
        │   │   └───node_modules
        │   │       ├───debug
        │   │       │   └───src
        │   │       ├───has-flag
        │   │       ├───ms
        │   │       └───supports-color
        │   ├───normalize-path
        │   ├───object-inspect
        │   │   ├───.github
        │   │   ├───example
        │   │   └───test
        │   │       └───browser
        │   ├───on-finished
        │   ├───parseurl
        │   ├───path-to-regexp
        │   ├───picomatch
        │   │   └───lib
        │   ├───proxy-addr
        │   ├───pstree.remy
        │   │   ├───lib
        │   │   └───tests
        │   │       └───fixtures
        │   ├───punycode
        │   ├───qs
        │   │   ├───.github
        │   │   ├───dist
        │   │   ├───lib
        │   │   └───test
        │   ├───range-parser
        │   ├───raw-body
        │   ├───readdirp
        │   ├───safe-buffer
        │   ├───safer-buffer
        │   ├───semver
        │   │   ├───bin
        │   │   ├───classes
        │   │   ├───functions
        │   │   ├───internal
        │   │   └───ranges
        │   ├───send
        │   │   └───node_modules
        │   │       ├───encodeurl
        │   │       └───ms
        │   ├───serve-static
        │   ├───set-function-length
        │   │   └───.github
        │   ├───setprototypeof
        │   │   └───test
        │   ├───side-channel
        │   │   ├───.github
        │   │   └───test
        │   ├───sift
        │   │   ├───es
        │   │   ├───es5m
        │   │   ├───lib
        │   │   └───src
        │   ├───simple-update-notifier
        │   │   ├───build
        │   │   └───src
        │   ├───sparse-bitfield
        │   ├───statuses
        │   ├───supports-color
        │   ├───to-regex-range
        │   ├───toidentifier
        │   ├───touch
        │   │   └───bin
        │   ├───tr46
        │   │   └───lib
        │   ├───type-is
        │   ├───undefsafe
        │   │   ├───.github
        │   │   │   └───workflows
        │   │   └───lib
        │   ├───unpipe
        │   ├───utils-merge
        │   ├───vary
        │   ├───webidl-conversions
        │   │   └───lib
        │   └───whatwg-url
        │       └───lib
        ├───public
        │   └───css
        └───views
            └───partials
```

## API Endpoints

| Method | Endpoint               | Description                          |
|--------|------------------------|--------------------------------------|
| GET    | /api/posts              | Fetch all blog posts                 |
| GET    | /api/posts/:id          | Fetch a single blog post by ID       |
| POST   | /api/posts              | Create a new blog post (Admin)       |
| PUT    | /api/posts/:id          | Edit a blog post (Admin)             |
| DELETE | /api/posts/:id          | Delete a blog post (Admin)           |

## How It Works

1. **Frontend**:  
   The frontend consists of static HTML, CSS, and JavaScript files.  The blog posts are dynamically displayed using JavaScript on the page.

2. **Backend**:  
   The backend is a RESTful API built with Node.js and Express.js, connected to a MongoDB database where blog posts are stored. The admin can send requests to create, update, or delete blog posts via HTTP requests.

## Contributions

Feel free to fork this project and submit pull requests. We welcome contributions that improve the project!

## License

This project is licensed under the Hardik License - see the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or feedback, please contact Hardik at [hardik.57v@gmail.com].
