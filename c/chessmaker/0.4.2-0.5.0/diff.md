# Comparing `tmp/chessmaker-0.4.2.tar.gz` & `tmp/chessmaker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.4.2.tar", max compression
+gzip compressed data, was "chessmaker-0.5.0.tar", max compression
```

## Comparing `chessmaker-0.4.2.tar` & `chessmaker-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,57 @@
--rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.4.2/chessmaker/__init__.py
--rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.4.2/chessmaker/chess/__init__.py
--rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.4.2/chessmaker/chess/base/__init__.py
--rw-r--r--   0        0        0     6811 2023-04-22 18:15:44.473745 chessmaker-0.4.2/chessmaker/chess/base/board.py
--rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.4.2/chessmaker/chess/base/game.py
--rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.4.2/chessmaker/chess/base/move_option.py
--rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.4.2/chessmaker/chess/base/piece.py
--rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.4.2/chessmaker/chess/base/player.py
--rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.4.2/chessmaker/chess/base/position.py
--rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.4.2/chessmaker/chess/base/rule.py
--rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.4.2/chessmaker/chess/base/square.py
--rw-r--r--   0        0        0     5281 2023-04-22 20:33:13.515140 chessmaker-0.4.2/chessmaker/chess/game_factory.py
--rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.4.2/chessmaker/chess/piece_utils.py
--rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.4.2/chessmaker/chess/pieces/__init__.py
--rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.4.2/chessmaker/chess/pieces/bishop.py
--rw-r--r--   0        0        0     7173 2023-04-22 22:31:36.777549 chessmaker-0.4.2/chessmaker/chess/pieces/king.py
--rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.4.2/chessmaker/chess/pieces/knight.py
--rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.4.2/chessmaker/chess/pieces/knook/__init__.py
--rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knook.py
--rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable.py
--rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.4.2/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.4.2/chessmaker/chess/pieces/pawn.py
--rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.4.2/chessmaker/chess/pieces/queen.py
--rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.4.2/chessmaker/chess/pieces/rook.py
--rw-r--r--   0        0        0      331 2023-04-22 19:21:15.298254 chessmaker-0.4.2/chessmaker/chess/results/__init__.py
--rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.4.2/chessmaker/chess/results/capture_all_pieces_to_win.py
--rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.4.2/chessmaker/chess/results/checkmate.py
--rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.4.2/chessmaker/chess/results/double_check_to_win.py
--rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.4.2/chessmaker/chess/results/no_captures_or_pawn_moves.py
--rw-r--r--   0        0        0      961 2023-04-24 20:44:49.437636 chessmaker-0.4.2/chessmaker/chess/results/repetition.py
--rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.4.2/chessmaker/chess/results/stalemate.py
--rw-r--r--   0        0        0      680 2023-04-22 19:21:15.309254 chessmaker-0.4.2/chessmaker/chess/results/standard_result.py
--rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.4.2/chessmaker/chess/rules/__init__.py
--rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.4.2/chessmaker/chess/rules/beta_decay.py
--rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.4.2/chessmaker/chess/rules/forced_en_passant.py
--rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.4.2/chessmaker/chess/rules/il_vaticano.py
--rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.4.2/chessmaker/chess/rules/king_cant_move_to_c2.py
--rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.4.2/chessmaker/chess/rules/knight_boosting.py
--rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.4.2/chessmaker/chess/rules/la_bastarda.py
--rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.4.2/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.4.2/chessmaker/chess/rules/siberian_swipe.py
--rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.4.2/chessmaker/clients/__init__.py
--rw-r--r--   0        0        0    18218 2023-04-24 20:46:07.131795 chessmaker-0.4.2/chessmaker/clients/pywebio_ui.py
--rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.4.2/chessmaker/cloneable.py
--rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.4.2/chessmaker/events/__init__.py
--rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.4.2/chessmaker/events/event.py
--rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.4.2/chessmaker/events/event_priority.py
--rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.4.2/chessmaker/events/event_publisher.py
--rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.4.2/LICENSE
--rw-r--r--   0        0        0     1098 2023-04-22 20:38:50.134595 chessmaker-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.4.2/README.md
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.5.0/chessmaker/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.5.0/chessmaker/chess/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.5.0/chessmaker/chess/base/__init__.py
+-rw-r--r--   0        0        0     6896 2023-04-29 20:29:37.214179 chessmaker-0.5.0/chessmaker/chess/base/board.py
+-rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.5.0/chessmaker/chess/base/game.py
+-rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.5.0/chessmaker/chess/base/move_option.py
+-rw-r--r--   0        0        0     3483 2023-04-29 12:24:05.009609 chessmaker-0.5.0/chessmaker/chess/base/piece.py
+-rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.5.0/chessmaker/chess/base/player.py
+-rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.5.0/chessmaker/chess/base/position.py
+-rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.5.0/chessmaker/chess/base/rule.py
+-rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.5.0/chessmaker/chess/base/square.py
+-rw-r--r--   0        0        0     5589 2023-05-19 23:46:03.030277 chessmaker-0.5.0/chessmaker/chess/game_factory.py
+-rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.5.0/chessmaker/chess/piece_utils.py
+-rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.5.0/chessmaker/chess/pieces/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.5.0/chessmaker/chess/pieces/bishop.py
+-rw-r--r--   0        0        0     1155 2023-05-19 23:50:27.094690 chessmaker-0.5.0/chessmaker/chess/pieces/duck.py
+-rw-r--r--   0        0        0     7243 2023-04-29 12:11:06.816563 chessmaker-0.5.0/chessmaker/chess/pieces/king.py
+-rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.5.0/chessmaker/chess/pieces/knight.py
+-rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.5.0/chessmaker/chess/pieces/knook/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.5.0/chessmaker/chess/pieces/knook/knook.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.5.0/chessmaker/chess/pieces/knook/knookable.py
+-rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.5.0/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.5.0/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.5.0/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.5.0/chessmaker/chess/pieces/pawn.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.5.0/chessmaker/chess/pieces/queen.py
+-rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.5.0/chessmaker/chess/pieces/rook.py
+-rw-r--r--   0        0        0      363 2023-05-19 23:47:47.243517 chessmaker-0.5.0/chessmaker/chess/results/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.5.0/chessmaker/chess/results/capture_all_pieces_to_win.py
+-rw-r--r--   0        0        0      466 2023-05-19 23:46:03.043276 chessmaker-0.5.0/chessmaker/chess/results/checkmate.py
+-rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.5.0/chessmaker/chess/results/double_check_to_win.py
+-rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.5.0/chessmaker/chess/results/no_captures_or_pawn_moves.py
+-rw-r--r--   0        0        0      320 2023-05-19 23:56:22.399681 chessmaker-0.5.0/chessmaker/chess/results/no_kings.py
+-rw-r--r--   0        0        0      963 2023-05-19 23:56:09.830191 chessmaker-0.5.0/chessmaker/chess/results/repetition.py
+-rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.5.0/chessmaker/chess/results/stalemate.py
+-rw-r--r--   0        0        0      750 2023-05-19 23:46:03.049274 chessmaker-0.5.0/chessmaker/chess/results/standard_result.py
+-rw-r--r--   0        0        0      382 2023-05-19 23:48:02.511230 chessmaker-0.5.0/chessmaker/chess/rules/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.5.0/chessmaker/chess/rules/beta_decay.py
+-rw-r--r--   0        0        0      908 2023-04-29 21:32:40.795238 chessmaker-0.5.0/chessmaker/chess/rules/duck_chess.py
+-rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.5.0/chessmaker/chess/rules/forced_en_passant.py
+-rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.5.0/chessmaker/chess/rules/il_vaticano.py
+-rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.5.0/chessmaker/chess/rules/king_cant_move_to_c2.py
+-rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.5.0/chessmaker/chess/rules/knight_boosting.py
+-rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.5.0/chessmaker/chess/rules/la_bastarda.py
+-rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.5.0/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.5.0/chessmaker/chess/rules/siberian_swipe.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.5.0/chessmaker/clients/__init__.py
+-rw-r--r--   0        0        0    18358 2023-05-19 23:50:27.089692 chessmaker-0.5.0/chessmaker/clients/pywebio_ui.py
+-rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.5.0/chessmaker/cloneable.py
+-rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.5.0/chessmaker/events/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.5.0/chessmaker/events/event.py
+-rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.5.0/chessmaker/events/event_priority.py
+-rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.5.0/chessmaker/events/event_publisher.py
+-rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1098 2023-04-29 21:02:54.790039 chessmaker-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2328 2023-05-19 23:54:33.882254 chessmaker-0.5.0/README.md
+-rw-r--r--   0        0        0     3422 1970-01-01 00:00:00.000000 chessmaker-0.5.0/PKG-INFO
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/base/__init__.py` & `chessmaker-0.5.0/chessmaker/chess/base/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/base/board.py` & `chessmaker-0.5.0/chessmaker/chess/base/board.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
             self.propagate_all(piece)
 
     def _on_after_move(self, _: AfterMoveEvent):
         next_player = next(self.turn_iterator)
         before_turn_change_event = BeforeTurnChangeEvent(self, next_player)
         self.publish(before_turn_change_event)
         if before_turn_change_event.cancelled:
+            self.turn_iterator = itertools.chain([next_player], self.turn_iterator)
             return
         self.current_player = before_turn_change_event.next_player
         self.publish(AfterTurnChangeEvent(self, self.current_player))
 
     def __getitem__(self, position: Position) -> Square | None:
         return self._squares[position.y][position.x]
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/base/game.py` & `chessmaker-0.5.0/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/base/piece.py` & `chessmaker-0.5.0/chessmaker/chess/base/piece.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                      BeforeCapturedEvent, AfterCapturedEvent)
 
 
 @event_publisher(*PIECE_EVENT_TYPES)
 class Piece(Cloneable, EventPublisher):
     def __init__(self, player: Player):
         super().__init__()
-        self._player = player
+        self.player = player
         self._board: Board = None
 
     def __repr__(self):
         return f"{self.__class__.__name__} ({self.player})"
 
     def get_move_options(self) -> Iterable[MoveOption]:
         move_options = self._get_move_options()
@@ -89,18 +89,14 @@
 
         self.publish(AfterMoveEvent(self, move_option))
 
     def on_join_board(self):
         pass
 
     @property
-    def player(self):
-        return self._player
-
-    @property
     def position(self):
         return self.board._get_piece_position(self)
 
     @property
     def board(self):
         if self._board is None:
             raise Exception("Piece is not on the board yet")
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/base/player.py` & `chessmaker-0.5.0/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/base/rule.py` & `chessmaker-0.5.0/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/base/square.py` & `chessmaker-0.5.0/chessmaker/chess/base/square.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/game_factory.py` & `chessmaker-0.5.0/chessmaker/chess/game_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from chessmaker.chess import results
 from chessmaker.chess.base.board import Board
 from chessmaker.chess.base.game import Game
 from chessmaker.chess.base.piece import Piece
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.square import Square
 from chessmaker.chess.pieces.bishop import Bishop
+from chessmaker.chess.pieces.duck import Duck
 from chessmaker.chess.pieces.king import King
 from chessmaker.chess.pieces.knight import Knight
 from chessmaker.chess.pieces.knook.knookable_knight import KnookableKnight
 from chessmaker.chess.pieces.knook.knookable_rook import KnookableRook
 from chessmaker.chess.pieces.pawn import Pawn
 from chessmaker.chess.pieces.queen import Queen
 from chessmaker.chess.pieces.rook import Rook
-from chessmaker.chess.results import stalemate, Repetition, NoCapturesOrPawnMoves, checkmate
+from chessmaker.chess.results import stalemate, Repetition, NoCapturesOrPawnMoves, checkmate, no_kings
 from chessmaker.chess.rules import ForcedEnPassant, KnightBoosting, OmnipotentF6Pawn, SiberianSwipe, IlVaticano, \
-    BetaDecay, KingCantMoveToC2, LaBastarda
+    BetaDecay, KingCantMoveToC2, LaBastarda, DuckChess
 
 
 class A:
     pass
 
 
 def create_game(
@@ -35,21 +36,23 @@
         il_vaticano: bool = False,
         beta_decay: bool = False,
         la_bastarda: bool = False,
         king_cant_move_to_c2: bool = False,
         vertical_castling: bool = False,
         double_check_to_win: bool = False,
         capture_all_pieces_to_win: bool = False,
+        duck_chess: bool = False,
 ):
     _knight = Knight
     _rook = Rook
     castling_directions = ((1, 0), (-1, 0))
     if vertical_castling:
         castling_directions = tuple(list(castling_directions) + [(0, 1), (0, -1)])
-    _king = lambda player: King(player, attackable=capture_all_pieces_to_win, castling_directions=castling_directions)
+    attackable = capture_all_pieces_to_win or duck_chess
+    _king = lambda player: King(player, attackable=attackable, castling_directions=castling_directions)
     if knooks:
         _knight = KnookableKnight
         _rook = KnookableRook
 
     white = Player("white")
     black = Player("black")
     turn_iterator = cycle([white, black])
@@ -96,23 +99,26 @@
         (knight_boosting, KnightBoosting()),
         (siberian_swipe, SiberianSwipe()),
         (il_vaticano, IlVaticano()),
         (king_cant_move_to_c2, KingCantMoveToC2()),
         (omnipotent_f6_pawn, OmnipotentF6Pawn(pawn=_pawn)),
         (la_bastarda, LaBastarda(pawn=_pawn)),
         (beta_decay, BetaDecay([_rook, Bishop, _pawn])),
+        (duck_chess, DuckChess()),
     ]:
         if enabled:
             rules.append(rule)
 
     result_functions = [stalemate, Repetition(3), NoCapturesOrPawnMoves(50)]
     if capture_all_pieces_to_win:
         result_functions.insert(0, results.capture_all_pieces_to_win)
     else:
-        result_functions.insert(0, checkmate)
+        if not duck_chess:
+            result_functions.insert(0, checkmate)
+        result_functions.insert(0, no_kings)
 
     if double_check_to_win:
         result_functions.insert(0, results.double_check_to_win)
 
     class GetResult:
         def __init__(self):
             self.result_functions = result_functions
@@ -125,15 +131,15 @@
 
     game = Game(
         board=Board(
             squares=[
                 [Square(piece_row[i](black)) for i in range(8)],
                 [Square(_pawn(black)) for _ in range(8)],
                 _empty_line(8),
-                _empty_line(8),
+                _empty_line(7) + [Square(Duck(white) if duck_chess else None)],
                 _empty_line(8),
                 _empty_line(8),
                 [Square(_pawn(white)) for _ in range(8)],
                 [Square(piece_row[i](white)) for i in range(8)],
             ],
             players=[white, black],
             turn_iterator=turn_iterator,
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/piece_utils.py` & `chessmaker-0.5.0/chessmaker/chess/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/king.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/king.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,22 @@
             for move_option in move_options:
                 if self.position in move_option.captures:
                     return True
         return False
 
     @contextmanager
     def _make_kings_attackable(self):
+        previous_states = {}
         for piece in self.board.get_pieces():
             if isinstance(piece, King):
+                previous_states[piece] = piece._attackable
                 piece._attackable = True
         yield
-        for piece in self.board.get_pieces():
-            if isinstance(piece, King):
-                piece._attackable = False
+        for piece, previous_state in previous_states.items():
+            piece._attackable = previous_state
 
     def _is_attacked_after_move(self, piece: Piece, move_option: MoveOption) -> bool:
         with self._make_kings_attackable():
             board_clone = self.board.clone()
         self_clone = board_clone[self.position].piece
         piece_clone = board_clone[piece.position].piece
         piece_clone.move(move_option)
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/knight.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/queen.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/pieces/rook.py` & `chessmaker-0.5.0/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/results/checkmate.py` & `chessmaker-0.5.0/chessmaker/chess/results/double_check_to_win.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from chessmaker.chess.base import Board
 from chessmaker.chess.pieces import King
-from chessmaker.chess.results.stalemate import stalemate
-
-
-def checkmate(board: Board) -> str | None:
-    is_stalemate = stalemate(board)
-    if is_stalemate:
-        current_player = board.current_player
-        player_pieces = list(board.get_player_pieces(current_player))
-
-        kings = [piece for piece in player_pieces if isinstance(piece, King)]
-        if not kings or all(king.is_attacked() for king in kings):
-            return f"Checkmate - {current_player.name} loses"
 
 
+def double_check_to_win(board: Board) -> str | None:
+    current_player = board.current_player
+    player_pieces = list(board.get_player_pieces(current_player))
+
+    kings = [piece for piece in player_pieces if isinstance(piece, King)]
+    for king in kings:
+        attacker_count = 0
+        position = king.position
+        for piece in board.get_pieces():
+            if piece.player != current_player:
+                for move_option in piece.get_move_options():
+                    if position in move_option.captures:
+                        attacker_count += 1
+                        break
 
+        if attacker_count >= 2:
+            return f"Double check - {current_player.name} loses"
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/results/no_captures_or_pawn_moves.py` & `chessmaker-0.5.0/chessmaker/chess/results/no_captures_or_pawn_moves.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/results/repetition.py` & `chessmaker-0.5.0/chessmaker/chess/results/repetition.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
                 elif square.piece is None:
                     position_hash += "Empty"
                 else:
                     position_hash += square.piece.__class__.__name__ + square.piece.player._id
 
         self.positions[position_hash] = self.positions.get(position_hash, 0) + 1
         if self.positions[position_hash] >= self.needed_repetitions:
-            return "Repetition - Draw"
+            return "Repetition - Draw"
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/results/standard_result.py` & `chessmaker-0.5.0/chessmaker/chess/results/standard_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from chessmaker.chess.base.board import Board
+from chessmaker.chess.results import no_kings
 from chessmaker.chess.results.checkmate import checkmate
 from chessmaker.chess.results.no_captures_or_pawn_moves import NoCapturesOrPawnMoves
 from chessmaker.chess.results.repetition import Repetition
 from chessmaker.chess.results.stalemate import stalemate
 
 
 class StandardResult:
     def __init__(self):
         self.results = [
+            no_kings,
             checkmate,
             stalemate,
             Repetition(),
             NoCapturesOrPawnMoves(),
         ]
 
     def __call__(self, board: Board):
```

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.5.0/chessmaker/chess/rules/beta_decay.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/forced_en_passant.py` & `chessmaker-0.5.0/chessmaker/chess/rules/forced_en_passant.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.5.0/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/king_cant_move_to_c2.py` & `chessmaker-0.5.0/chessmaker/chess/rules/king_cant_move_to_c2.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.5.0/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/la_bastarda.py` & `chessmaker-0.5.0/chessmaker/chess/rules/la_bastarda.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.5.0/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.5.0/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.5.0/chessmaker/clients/pywebio_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,15 +407,15 @@
                           value="Singleplayer"),
                     actions("-", [
                         {"label": "Create", "value": "create"},
                     ], name="action"),
                 ])
                 shared_position = shared_positions[get_query("position_id")]
                 new_game(lambda **_: Game(shared_position.board.clone(), deepcopy(shared_position.get_result)),
-                            shared_position.options, form_result["mode"], piece_urls)
+                         shared_position.options, form_result["mode"], piece_urls)
             return
 
         form_result = input_group("New Game", [
             radio("Mode", ["Singleplayer", "Multiplayer (Private)", "Multiplayer (Public)"], name="mode",
                   value="Singleplayer"),
             checkbox(
                 "Options",
@@ -443,11 +443,14 @@
 
 
 if __name__ == "__main__":
     start_pywebio_chess_server(
         create_game,
         supported_options=["chess960", "knooks", "forced_en_passant", "knight_boosting", "omnipotent_f6_pawn",
                            "siberian_swipe", "il_vaticano", "beta_decay", "la_bastarda", "king_cant_move_to_c2",
-                           "vertical_castling", "double_check_to_win", "capture_all_pieces_to_win"],
-        piece_urls=PIECE_URLS | {"Knook": ["https://i.imgur.com/UiWcdEb.png", "https://i.imgur.com/g7xTVts.png"]}
-        ,remote_access=True, debug=True
+                           "vertical_castling", "double_check_to_win", "capture_all_pieces_to_win", "duck_chess"],
+        piece_urls=PIECE_URLS |
+                   {
+                       "Knook": ["https://i.imgur.com/UiWcdEb.png", "https://i.imgur.com/g7xTVts.png"],
+                       "Duck": ["https://i.imgur.com/ZZ2WSUq.png", "https://i.imgur.com/ZZ2WSUq.png"]
+                   }
     )
```

### Comparing `chessmaker-0.4.2/chessmaker/events/event_publisher.py` & `chessmaker-0.5.0/chessmaker/events/event_publisher.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/LICENSE` & `chessmaker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.2/pyproject.toml` & `chessmaker-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chessmaker"
-version = "0.4.2"
+version = "0.5.0"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = ["WolfDWyc <yoavwolfdw@gmail.com>",]
 license = "AGPL-3.0-or-later"
 classifiers = [
 "License :: OSI Approved :: GNU Affero General Public License v3",
 "Programming Language :: Python",
```

### Comparing `chessmaker-0.4.2/README.md` & `chessmaker-0.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -14,39 +14,43 @@
 ---
 
 ## What is ChessMaker?
 
 ChessMaker is a Python (3.11+) chess implementation that can be extended to support any custom rule or feature.
 It allows you to build almost any variant you can think of easily and quickly.
 
-ChessMaker isn't tied to any GUI, but comes with a thin, [pywebio](https://pywebio.readthedocs.io/en/latest/), multiplayer web interface.
-
 It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the packaged optional rules are almost all inspired by that subreddit.
 
-These rules are:
+ChessMaker isn't tied to any GUI, but comes with a thin, [pywebio](https://pywebio.readthedocs.io/en/latest/), multiplayer web interface.
+The web interface supports choosing from the packaged rules, singleplayer (vs Yourself), and multiplayer
+(vs a friend or random opponent). It also supports saving and loading games - which can be shared with others
+and be used as puzzles.
+
+The packaged rules are:
 
 * Chess960
 * Knooks
 * Forced En Passant
 * Knight Boosting
 * Siberian Swipe
 * Il Vaticano
 * Beta Decay
 * La Bastarda
 * Omnipotent F6 Pawn
 * King Cant Move to C2
 * Vertical Castling
 * Double Check to Win
 * Capture All Pieces to Win
+* Duck Chess
 
+Contributions of new variants or anything else you'd like to see in the project are welcome!
 
 ## What ChessMaker isn't
 
-* A complete chess server - It doesn't support users, matchmaking, ratings, cheating detection, etc. 
-The frontend is very simple and not the focus of the project.
-* A chess engine. The design choices are not optimized for speed, and it doesn't provide any analysis or AI.
-* A compliant or standard chess implementation. It doesn't support UCI or existing chess GUIs,
+* A complete chess server - It currently doesn't support users, matchmaking, ratings, cheating detection,
+and is very thin. The frontend is very simple and currently not the focus of the project.
+* A chess engine - The design choices are not optimized for speed, and it doesn't provide any analysis or AI.
+* A compliant or standard chess implementation - It doesn't support UCI or existing chess GUIs,
 because it allows rules that wouldn't be possible with those.
 
-Note: While ChessMaker isn't a chess server, one could be built on top of it, and development of alternative clients to it is welcomed and encouraged.
-
-
+-Note: While ChessMaker isn't a chess server, one could be built on top of it, and development of alternative clients to it is welcomed and encouraged.
+If this project gets enough interest, a more complete server might be added.
```

### Comparing `chessmaker-0.4.2/PKG-INFO` & `chessmaker-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.4.2
+Version: 0.5.0
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 License: AGPL-3.0-or-later
 Keywords: chess
 Author: WolfDWyc
 Author-email: yoavwolfdw@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -40,40 +40,44 @@
 ---
 
 ## What is ChessMaker?
 
 ChessMaker is a Python (3.11+) chess implementation that can be extended to support any custom rule or feature.
 It allows you to build almost any variant you can think of easily and quickly.
 
-ChessMaker isn't tied to any GUI, but comes with a thin, [pywebio](https://pywebio.readthedocs.io/en/latest/), multiplayer web interface.
-
 It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the packaged optional rules are almost all inspired by that subreddit.
 
-These rules are:
+ChessMaker isn't tied to any GUI, but comes with a thin, [pywebio](https://pywebio.readthedocs.io/en/latest/), multiplayer web interface.
+The web interface supports choosing from the packaged rules, singleplayer (vs Yourself), and multiplayer
+(vs a friend or random opponent). It also supports saving and loading games - which can be shared with others
+and be used as puzzles.
+
+The packaged rules are:
 
 * Chess960
 * Knooks
 * Forced En Passant
 * Knight Boosting
 * Siberian Swipe
 * Il Vaticano
 * Beta Decay
 * La Bastarda
 * Omnipotent F6 Pawn
 * King Cant Move to C2
 * Vertical Castling
 * Double Check to Win
 * Capture All Pieces to Win
+* Duck Chess
 
+Contributions of new variants or anything else you'd like to see in the project are welcome!
 
 ## What ChessMaker isn't
 
-* A complete chess server - It doesn't support users, matchmaking, ratings, cheating detection, etc. 
-The frontend is very simple and not the focus of the project.
-* A chess engine. The design choices are not optimized for speed, and it doesn't provide any analysis or AI.
-* A compliant or standard chess implementation. It doesn't support UCI or existing chess GUIs,
+* A complete chess server - It currently doesn't support users, matchmaking, ratings, cheating detection,
+and is very thin. The frontend is very simple and currently not the focus of the project.
+* A chess engine - The design choices are not optimized for speed, and it doesn't provide any analysis or AI.
+* A compliant or standard chess implementation - It doesn't support UCI or existing chess GUIs,
 because it allows rules that wouldn't be possible with those.
 
-Note: While ChessMaker isn't a chess server, one could be built on top of it, and development of alternative clients to it is welcomed and encouraged.
-
-
+-Note: While ChessMaker isn't a chess server, one could be built on top of it, and development of alternative clients to it is welcomed and encouraged.
+If this project gets enough interest, a more complete server might be added.
```

