# SEEM3650 Practical Exam Report

Name: Mak Loren Tsz Long 
Student ID: 1155212355

## Step 2: Shakespeare Character-level Samples

```text
And they bring with the sorrow
They was be a enamier'd with tale
My arm that us and to bar distion.

First Citizen:
```


## Step 3: Model Architecture Exploration

My student ID is 1155212355, so the last three digits are XYZ = 355.

Since 355 mod 4 = 3, I fixed `n_head = 4` and tested `n_layer = 2, 3, 5, and 7`.

I used a reduced configuration on Google Colab to keep training time manageable.

The loss was measured using validation loss at step 1000.

| Run | Layers | Heads | Train Loss | Validation Loss |
|---|---:|---:|---:|---:|
| 1 | 2 | 4 | 1.7169 | 1.8746 |
| 2 | 3 | 4 | 1.6877 | 1.8454 |
| 3 | 5 | 4 | 1.6002 | 1.766 |
| 4 | 7 | 4 | 1.5517 | 1.7121 |

The lowest validation loss I achieved was 1.7121.

The best setting on my machine was:

- Layers: 7
- Heads: 4

The corresponding figure is saved as `figures/loss_vs_layers.png`.


## Step 4: Code Generation

Since 355 mod 2 = 1, I used Python open-source code for the code generation dataset.

The number of tokens in my code generation dataset is: 2540758.

I trained the code generation model for 1000 iterations using a reduced configuration on Google Colab.

## First 20 lines of generated code samples

```text
Overriding: out_dir = out-code-generation
number of parameters: 0.81M
Loading meta from data/code_generation/meta.pkl...

        flask.upden_bool_name = request,
        "":class[x.Command(Commannd()], [0], False),
        [("-c"], "--http: flamb", "f"", "rp", "byte", {"help": "-valomt", "flag_ver_filed":"1
        ({
         ["----f-domaial",
        ("f"wor": "thest", {"dot": "default", "True": 3"),
         ({"test_data="pplsec-default=default!2",
             " ``````_line``` apple.wordir
        " response.add_fule is gnot and be option in can actor" and
                                                      
---------------

        :param doptionrt: The able processe of basic iviable versions function the index bate. If the
        for file set to default the body a offfiname in threception other applies.

    .. command():

```

## Favorite generated snippet

```text
Overriding: out_dir = out-code-generation
number of parameters: 0.81M
Loading meta from data/code_generation/meta.pkl...

        flask.upden_bool_name = request,
        "":class[x.Command(Commannd()], [0], False),
        [("-c"], "--http: flamb", "f"", "rp", "byte", {"help": "-valomt", "flag_ver_filed":"1
        ({
         ["----f-domaial",
        ("f"wor": "thest", {"dot": "default", "True": 3"),
         ({"test_data="pplsec-default=default!2",
             " ``````_line``` apple.wordir
        " response.add_fule is gnot and be option in can actor" and
                                                      
---------------

        :param doptionrt: The able processe of basic iviable versions function the index bate. If the
        for file set to default the body a offfiname in threception other applies.

    .. command():
         (
               True
                   self.aborter = app

    def htt is_called_app(dovwary_signmest_parame_environ):
           elst"Bluep the filed to in the conect imported the turn
    cappecates the faund to the app.

    :param objs to_condex_parame_error` if the i) ais the to 
---------------

                 raise None
                        request.headers().max_html(preq_state))

              def rvion_func_get_sult():
                         assert arguo_match() is self._command.append()
                      ["-Reporce"] == "-"\n"

                    assert.parame(f"_ause") == [?mestame).path
                                     )

```
