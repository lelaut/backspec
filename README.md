# Backspec

A tool for building a **Specification-Driven API**.

### How it works

**On creating a specification repository**

1. Push Swagger spec fle
2. Push `README.md`(following a template) file
3. Push our Github Actions called `action.yaml`

**On client repository**

1. Add _client repository reference_ to Spec Repo `README.md` file

### What does each action do

- `action.yaml`:
  - Create a Swagger Server
  - When a change to the spec file happens it will create an `PullRequest` for each client repo containing the changes
  - When a new client is added to the `README.md` it will push the spec-client code to the client-repo

### References

- [Swagger](https://github.com/swagger-api)
- [Github Actions](https://github.com/features/actions)
- [Visualize infra with diagrams](https://www.cloudcraft.co/)
