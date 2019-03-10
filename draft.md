## Agenda
1. Sync vs Async
2. Callbacks
3. Promises
4. Generators
5. Await/async

## Sync vs Async
### Event loop
- definition (RFC ?)
- Parallel vs async (simultaneously vs later, after an undefined amount of time)
- List of tasks executed in sequence
    - No parallel access or update to shared memory
- Run-to-completion
- Race conditions only at function level
- Event loop tasks are executed one by one
- if encounter async callback, insert it into the task queue when ready

### Our brain is synchronous
- High level thinking is synchronous, single tasked
- If faking multitasking, lose focus ; actually quickly switching from one task to another
- Do tasks one after the another, step by step, each step blocking the next one
- Our brain = event loop

### Sync code vs async code
- Easy to read
- Order straightforward

## Callback hell
- definition (héhéhé)
    - code nesting
    - execution order (full async, mixed, don't know)
    - complex workflows
    - cover too early, too late, never, too many times ?

## Promise
- definition
- how it works
- what problem does it solve ?

## Generators
- definition
- how it works
- what problem does it solve ?

## Promise + generators = async / await
- Write async code ... in a synchronous way !!!! OMG !!!
- Composition, small functions
- Clean code
- Error output
- Debugging

=> async code less obvious ... WTF !!!

https://hackernoon.com/6-reasons-why-javascripts-async-await-blows-promises-away-tutorial-c7ec10518dd9