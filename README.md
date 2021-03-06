# Alexa + Amazon AWS Lambda Starter Kit (Node.js 6.x.x)
------
This will offer everything you need to get started on Amazon's ASK with an AWS Lambda backend.

### The Goal:
 - Get your Skill up and running ASAP
 - Give a generic structure that you can build upon
 - Offer documentation in the codebase and tests to aid with comprehension

### What's included:
 - Eslint - to keep your code consistent
 - Mocha & Chai - to test your code
 - Sinon - for better functional testing
 - Joi - self documenting schema to make sure your requests and responses are valid

### Getting Started: (This will probably change)
 1. `git clone https://github.com/brewencoded/alexa-lambda-starter.git`
 2. `cd alexa-lambda-starter`
 3. `npm install`

**To test**: `npm run test`

**To build**: `npm run build` *WIP*

**To deploy**: `npm run publish` *WIP*

If you have not set up the AWS CLI, [click here](https://developer.amazon.com/blogs/post/Tx1UE9W1NQ0GYII/publishing-your-skill-code-to-lambda-via-the-command-line-interface) for detailed instructions.

Now you're ready to get started. The build script will produce what is to be uploaded to AWS Lambda. Make sure when you create a Lambda, that you select the "Alexa Skill Kit" trigger.

Make sure to modify the [publish.sh](https://github.com/brewencoded/alexa-lambda-starter/blob/master/publish.sh#L5) to reflect **your** Lambda function's name. If you're on Windows replace `rm` with `del` and replace the zip line with your preferred utility. You will get an error on the first run since the zip file doesn't exist yet.

### TODO
- [X] Mocha and Chai
- [X] Sinon
- [X] Eslint
- [ ] `--fix` to automatically fix simple issues
- [X] Joi validation
- [X] Testing scripts
- [X] Response schema validation
- [ ] Request schema validation
- [ ] Intent schema
- [ ] Sample utterances
- [ ] Slots
- [ ] Code coverage
- [ ] Build scripts
- [ ] Deploy scripts
- [ ] Add Continuous Integration
- [ ] Docker Support
