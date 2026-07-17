# To Do

- [ ] **thebloom: gate the Keeper's Reference docs.** `run_worker_first` in
      `thebloom/wrangler.jsonc` only intercepts `/keeper.html` and `/keeper`
      for the login check. `The-Blooming-Keepers-Reference.docx`/`.pdf` (and
      anything else served from the same public asset root) bypass auth
      entirely via a direct link/URL guess. Either add those paths to
      `run_worker_first`, or move the files somewhere the worker gates before
      falling back to assets.
