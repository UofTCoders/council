
# Steps to get reimbursed

1. Get your GitHub account [GPG verified](https://help.github.com/categories/gpg/) 
(if you need help with that, come to a session and we'll get it set up)
2. Fork the council repo and clone it to your computer, then follow these
instructions:
    1. Copy `treasurer/reimbursing/template.md` to the `treasurer/reimbursing/submitted/` directory.
    2. Rename the file to `YYYY-MM-DD-firstname-lastname.md`: YYYY = year, MM =
    month, DD = day (all numbers), and firstname + lastname = your first and last name.
    3. Replace the relevant details to the file.
    4. Add and commit the file, push to your repo, and submit a pull request.
    5. Copy the pull request link to the file in the appropriate location.
    6. Commit and push the added change.
    - Or in the shell:
        ```
        cd treasurer/reimbursing
        mkdir submitted # if submitted doesn't exist
        cp template.md submitted/YYYY-MM-DD-firstname-lastname.md
        cd submitted
        # edit new file details
        git add YYYY-MM-DD-firstname-lastname.md 
        git commit -S -m "Added reimbursement claim form" # -S is for the GPG signing
        git push origin master
        # Submit a pull request on Github and add the link to the submitted md file
        git add YYYY-MM-DD-firstname-lastname.md 
        git commit -S -m "Added Github PR link to reimbursing details" # -S is for GPG signing
        git push origin master
        ```
3. (Optional) Scan your receipts, add them to the `receipts/` directory, and
submit them with your pull request.
4. Get your Pull Request approved by at least two other council excutives.
5. **(Required)** give the receipts to the treasurer.
6. Either meet up with the treasurer to get your cheque or whenever next you see
the treasurer (or who ever has the cheque).
