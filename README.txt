OR-Tools - Sudoku Solver - 

Ce code implémente une classe nomé : OrToolsSolver
et implemente l'interface : ISudokuSolver

pour résoudre un sudoku il suffit d'appeler la méthode : 

Sudoku Solve(Sudoku s)

cette méthode retourne le sudoku résolu. 

Exemple: 
	int[] initial_grid = new int[] { 0, 6, 0, 0, 5, 0, 0, 2, 0,

                                             0, 0, 0, 3, 0, 0, 0, 9, 0,

                                             7, 0, 0, 6, 0, 0, 0, 1, 0,

                                             0, 0, 6, 0, 3, 0, 4, 0, 0,

                                             0, 0, 4, 0, 7, 0, 1, 0, 0,

                                             0, 0, 5, 0, 9, 0, 8, 0, 0,

                                             0, 4, 0, 0, 0, 1, 0, 0, 6,

                                             0, 3, 0, 0, 0, 8, 0, 0, 0,

                                             0, 2, 0, 0, 4, 0, 0, 5, 0 };
	//création d'un sudoku 
 	Noyau.Sudoku s = new Noyau.Sudoku(initial_grid);
        Console.WriteLine(s.ToString());
	
	//création du solveur
        OrToolsSolver ORT = new OrToolsSolver();
        s = ORT.Solve(s);
        Console.WriteLine(s.ToString());


cette méthode prend en paramètre un objet Sudoku qui permet de générer un sudoku.
cf:README de la classe Sudoku



