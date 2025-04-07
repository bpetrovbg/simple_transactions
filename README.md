## Getting Started

### Prerequisites

Ensure you have the following installed on your machine:

- [Node.js LTS](https://nodejs.org/en)
- [Rush](https://rushjs.io/)

### Setting Up the Project

1. **Clone the Repository**

   Before cloning, please ensure you understand and agree to the terms of the GNU Affero General Public License as outlined in the LICENSE file. By cloning or forking the repository, you agree to comply with the license terms.

   ```bash
   git clone https://github.com/bpetrovbg/simple_transactions
   ```

2. **Install Dependencies**

   Use Rush to install and link all dependencies across the monorepo:

   ```bash
   rush install
   ```

3. **Update Libraries**

   If you add or change any node modules, make sure to update the libraries using:

   ```bash
   rush update
   ```

### Development Workflow

To start development, you will need to open two command prompts (CMDs):

1. **In the Root Folder**

   In the first CMD, navigate to the root folder of the project and run one of the following commands:

   - To watch for changes and build all projects:

     ```bash
     rush build:watch
     ```

   - To watch for changes and build all projects except a specific library:

     ```bash
     rush build:watch --to-except <library-name>
     ```

2. **In the Specific Frontend**

   In the second CMD, navigate to the specific frontend you are working on and run:

   ```bash
   rushx start
   ```

This will start the development server for the frontend application you are working on.

Please remember that any modifications or distributions of the code must adhere to the terms specified in the LICENSE file.
